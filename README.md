# Gerenciamento de Salas
Aplicação desenvolvida com a finalidade de auxiliar no gerenciamento de salas dentro de uma organização, onde será possível ter uma gestão mais completa e assertiva sobre as locações e disponibilidade de cada uma delas.

# Instalação para rodar em ambiente local

Python:  sudo apt-get install python3
<br>
Flask: pip install Flask 
<br>
pip install -U flask-cors
<br>
pip install flask-mysql
<br>
Rest Client
<br>
Banco de dados Mysql

# Configuração Banco de dados MySQL

Para criarmos nossa tabela iremos utilizar a Query:

CREATE TABLE `room` (
`id` int(11) NOT NULL,
`name` varchar(255) DEFAULT NULL,
`capacity` smallint(6) NOT NULL,
`start` timestamp NULL DEFAULT current_timestamp(),
`end` timestamp NULL DEFAULT current_timestamp()
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4;

<br><br>
Pra Inserirmos nossa base dentro da tabela iremos utilizar a Query:
<br>

INSERT INTO `room` (`id`, `name`, `capacity`, `start`, `end`) VALUES
(1, 'Sala 1', 5, '2022-05-21 21:00:00', '2022-05-22 17:00:00'),
(2, 'Sala 2', 50, '2022-05-21 21:00:00', '2022-05-22 17:00:00'),
(3, 'Sala 3', 150, '2022-05-19 11:00:00', '2022-05-21 21:00:00'),
(4, 'Sala 4', 75, '2022-05-19 11:00:00', '2022-05-21 21:00:00');
<br><br>

# Requirements

click==8.1.3
<br>
colorama==0.4.4
<br>
Flask==2.1.2
<br>
Flask-Cors==3.0.10
<br>
Flask-MySQL==1.5.2
<br>
itsdangerous==2.1.2
<br>
Jinja2==3.1.2
<br>
MarkupSafe==2.1.1
<br>
PyMySQL==1.0.2
<br>
six==1.16.0
<br>
Werkzeug==2.1.2


# Funcionalidades


1-	Cadastro de sala: A funcionalidade de cadastro de sala permite ser realizado o cadastro de sua sala existente dentro de sua organização, contendo o nome dado para a sala e sua capacidade máxima de pessoas.

2-	Lista de salas: Através desta funcionalidade é possível verificar todas as salas cadastradas juntamente com seu nome, capacidade e datas caso esteja alugada.

3-	Busca de salas: Através desta funcionalidade é possível localizar uma sala através de seu nome e também por disponibilidade.

4-	Agendamento de sala: Através da funcionalidade de agendamento é possível realizar o agendamento da sala desejada marcando também o horário de utilização, para que não ocorra conflitos ao reservar a sala. 

# Documentação API

<a href="http://documentacao.paulocrisci.com.br">Clique aqui para ver a documentação!</a></li>
