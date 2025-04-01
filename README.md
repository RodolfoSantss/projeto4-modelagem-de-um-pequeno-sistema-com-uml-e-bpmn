# PROJETO-4-MODELAGEM-DE-UM-PEQUENO-SISTEMA-COM-UML-E-BPMN

equipe: ARIEL & RODOLFO

## "BPMN"

[INÍCIO] -> [usuário acessa o sistema] -> [seleciona sala e horário] -> [verifica disponibilidade] -> {sala disponível?} <br>
    -> [SIM] -> [reserva confirmada] -> [FIM] <br>
    -> [NÃO] -> [exibe salas alternativas] -> [FIM] <br>

## "UML"

/=======================/ <br>
	CLIENTE <br>
/=======================/ <br>
	- nome: String <br>
	- email: String <br>
/=======================/ <br>
	 agendarSala() <br>
/=======================/ <br>
 <br>
Cliente 1 === 0 (false) <br>
Cliente 1 === 1 (true) --------------| <br>
				     | <br>
/=======================/	     | <br>
	SALA			    <| <br>
/=======================/ <br>
	# fazerReserva <br>
/=======================/ <br>
reserva [+ local() <br>
	+ data() <br>
	+ horário()] <br>
/=======================/ <br>
	reserva 1 === 0 (false) <br>
	reserva 1 === 1 (true) -------------| <br>
					    | <br>
			 Espaço agendado.  <| <br>
