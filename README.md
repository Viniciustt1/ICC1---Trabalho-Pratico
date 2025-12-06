# Sistema de Gerenciamento de Jogos e Atletas - Atlética CAASO
  Este repositório contém o código-fonte para um sistema de gerenciamento de eventos esportivos, atletas e confrontos, desenvolvido para auxiliar a organização de competições da Atlética CAASO.

# Funcionalidades Principais
O sistema é um aplicativo de console (CLI) em Python que permite:

1) Cadastro de Usuários:
  * Registro de Atletas com informações de contato, modalidade de interesse e secretaria acadêmica;
  * Registro de Administradores com chave de acesso.
    
2) Gestão de Dados:
  * Importação em massa de dados de Atletas via arquivo Excel (.xlsx);
  * Importação de Disponibilidade de Times a partir de planilhas de horários.
    
3) Gestão de Confrontos:
  * Criação de Chaveamento e Agendamento de jogos;
  * Alocação de times e definição de confrontos (incluindo byes);
  * Registro de Placar Detalhado e definição do time Vencedor.
    
4) Relatórios:
  * Visualização de atletas, confrontos e agenda;
  * Geração de relatórios de quórum e disponibilidade.

# Estrutura do Código
O código é estruturado em classes para representar as entidades principais e funções para as operações de CRUD (Criação, Leitura, Atualização, Deleção) e importação de dados:

  - Classes: Administrador, Atleta, Confronto.
  - Módulos:
    * CONFIGURAÇÕES E SEGURANÇA: Definição de constantes e função de login;
    * BANCOS DE DADOS: Dicionários e listas para simular o armazenamento de dados (BIBLIOTECA_ATLETAS, AGENDA, etc.);
    * FUNÇÕES DE IMPORTAÇÃO (PANDAS): Funções que utilizam a biblioteca pandas para ler dados de arquivos Excel;
    * FUNÇÕES DE CRUD (MANUAL): Funções para cadastro e edição manual de entidades;
    * FUNÇÕES DE GESTÃO DE CONFRONTOS: Lógica para chaveamento, agendamento e registro de resultados;
    * MENU PRINCIPAL: Interface de linha de comando para interação com o usuário.
