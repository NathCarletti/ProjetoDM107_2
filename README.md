# ProjetoDM107_2
WebService with Security using Java, Gradle, Jersey and PHP


DataBase:

CREATE DATABASE IF NOT EXISTS `servicodb`;

USE `servicodb`;
CREATE TABLE IF NOT EXISTS `entregadb` (
`id` integer NOT NULL auto_increment,
`idCliente` integer NOT NULL,
`numPedido` integer NOT NULL,
`numPedido` varchar(50) NOT NULL default '',
`cpfRecebidor` varchar(50) NOT NULL default '',
`dataHoraEntrega` varchar(50) NOT NULL default '',
PRIMARY KEY (`id`),
);

USE `servicodb`;
CREATE TABLE IF NOT EXISTS `usuariodb` (
`id` integer NOT NULL auto_increment,
`usuario` varchar(50) NOT NULL default '',
`senha` varchar(50) NOT NULL default '',
PRIMARY KEY (`id`),
);
