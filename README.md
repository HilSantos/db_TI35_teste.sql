# db_TI35_teste.sql
Teste do Banco de Dados Alunos

-- phpMyAdmin SQL Dump
-- version 5.2.1
-- https://www.phpmyadmin.net/
--
-- Host: 127.0.0.1
-- Tempo de geração: 17/02/2025 às 17:54
-- Versão do servidor: 10.4.32-MariaDB
-- Versão do PHP: 8.2.12

SET SQL_MODE = "NO_AUTO_VALUE_ON_ZERO";
START TRANSACTION;
SET time_zone = "+00:00";


/*!40101 SET @OLD_CHARACTER_SET_CLIENT=@@CHARACTER_SET_CLIENT */;
/*!40101 SET @OLD_CHARACTER_SET_RESULTS=@@CHARACTER_SET_RESULTS */;
/*!40101 SET @OLD_COLLATION_CONNECTION=@@COLLATION_CONNECTION */;
/*!40101 SET NAMES utf8mb4 */;

--
-- Banco de dados: `db_ti35_teste`
--
CREATE DATABASE IF NOT EXISTS `db_ti35_teste` DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_general_ci;
USE `db_ti35_teste`;

-- --------------------------------------------------------

--
-- Estrutura para tabela `tb_alunos`
--

DROP TABLE IF EXISTS `tb_alunos`;
CREATE TABLE `tb_alunos` (
  `id_aluno` int(11) NOT NULL,
  `nome_aluno` varchar(80) DEFAULT NULL,
  `telefone_aluno` varchar(14) DEFAULT NULL,
  `email_aluno` varchar(40) DEFAULT NULL,
  `cpf_aluno` varchar(11) DEFAULT NULL,
  `endereco_aluno` varchar(80) DEFAULT NULL,
  `nascimento_aluno` date DEFAULT NULL,
  `mensalidade_aluno` decimal(7,2) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
-- Despejando dados para a tabela `tb_alunos`
--

INSERT INTO `tb_alunos` (`id_aluno`, `nome_aluno`, `telefone_aluno`, `email_aluno`, `cpf_aluno`, `endereco_aluno`, `nascimento_aluno`, `mensalidade_aluno`) VALUES
(2, 'Paulo Castro', '5516994037928', 'silvasantos1933@proton.me', '88534521099', 'Av. Washington Luis, 777', '1984-03-22', 160.00),
(3, 'Louis Johanson', '5511994037928', 'usuario@admin.com.br', '02096618344', 'R. Voluntarios da Patria, 113', '1978-12-04', 25.00),
(4, 'Mike Dismore', '5516988031205', 'dismorem@yahoo.com', '67720154032', 'Av. Profº Francisco Morato, 2237', '1933-12-30', 210.00),
(5, 'Irene Cara', '5511997015643', 'carairene@outlook.com', '33179051288', 'R. Frei Durão, 76', '2001-06-01', 63.00),
(6, 'Maria de Lourdes Silva', '5511988471234', 'silvalouma@hotmail.com', '09125842100', 'Av. do Cursino, 61', '2013-09-17', 40.00);

--
-- Índices para tabelas despejadas
--

--
-- Índices de tabela `tb_alunos`
--
ALTER TABLE `tb_alunos`
  ADD PRIMARY KEY (`id_aluno`);

--
-- AUTO_INCREMENT para tabelas despejadas
--

--
-- AUTO_INCREMENT de tabela `tb_alunos`
--
ALTER TABLE `tb_alunos`
  MODIFY `id_aluno` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=7;
COMMIT;

/*!40101 SET CHARACTER_SET_CLIENT=@OLD_CHARACTER_SET_CLIENT */;
/*!40101 SET CHARACTER_SET_RESULTS=@OLD_CHARACTER_SET_RESULTS */;
/*!40101 SET COLLATION_CONNECTION=@OLD_COLLATION_CONNECTION */;
