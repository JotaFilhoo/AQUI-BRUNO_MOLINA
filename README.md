Este é um projeto executado como prova no curso de ADS utilizando a linguagem JAVA. 
O programa tem como como objetivo fazer login, executar o CRUD por completo, cadastrando pacientes e nutricionistas.

Esta foi minha primeira tentativa de realização de um CRUD, também meu primeiro contato com banco de dados.


# Estrutura do banco de dados

-- Banco de dados: `projeto`
--

-- --------------------------------------------------------

--
-- Estrutura para tabela `login`
--

CREATE TABLE `login` (
  `id` int(11) NOT NULL,
  `username` varchar(16) NOT NULL,
  `senha` varchar(15) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;



-- --------------------------------------------------------

--
-- Estrutura para tabela `nutricionista`
--

CREATE TABLE `nutricionista` (
  `id` int(11) NOT NULL,
  `nome` varchar(20) NOT NULL,
  `crn` int(10) NOT NULL,
  `horario` varchar(10) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;


-- --------------------------------------------------------

--
-- Estrutura para tabela `paciente`
--

CREATE TABLE `paciente` (
  `id` int(11) NOT NULL,
  `nome` varchar(20) NOT NULL,
  `cpf` varchar(16) NOT NULL,
  `idade` int(11) NOT NULL,
  `peso` double NOT NULL,
  `altura` int(11) NOT NULL,
  `tmb` double NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

--
