ИС "Автоматизированная система кредитования юридических лиц".

Скрипт создания БД:

	CREATE TABLE loan_db.legal_entities (
	entitie_id int PRIMARY KEY NOT NULL, 
	en_name varchar(150) NOT NULL,
	address varchar(350) NOT NULL,
	phone_number varchar(20)
	)	


	CREATE TABLE loan_db.loans (
	loan_id int  PRIMARY KEY NOT NULL,
	entitie_id int NOT NULL,
	amount int NOT NULL, 
	percent float NOT NULL, 
	term int NOT NULL
	)