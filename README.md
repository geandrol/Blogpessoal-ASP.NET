BlogPessoal-ASP.NET

Um projeto em ASP.NET Core para um blog pessoal, com estrutura MVC, validação, serviços e configuração completa para desenvolvimento rápido e organizado.

Índice

Sobre

Funcionalidades

Tecnologias

Estrutura do Projeto

Instalação & Execução

Configuração

Boas Práticas

Contribuição

Licença

Sobre

Este projeto implementa um blog pessoal utilizando ASP.NET Core, organizado por camadas (Controllers, Models, Services, Validators). Ideal para quem busca uma base sólida para criar blogs e APIs web com boas práticas.

Funcionalidades

Estrutura MVC bem definida (Models, Controllers, Views ou API).

Camada de Serviços, para lógica de negócio centralizada.

Validação com classes dedicadas para garantir integridade de dados.

Configuração sensível ao ambiente (appsettings.json, appsettings.Development.json).

Projeto pronto para expansão com autenticação, banco de dados, testes, etc.

Tecnologias

.NET (versão usada no projeto) (insira a versão exata — ex: .NET 7, .NET 8)

ASP.NET Core

C#

[Adicione outras tecnologias ou pacotes conforme utilizados: Entity Framework Core, AutoMapper, etc.]

Estrutura do Projeto
/BlogPessoal-ASP.NET
│
├── Controller/            → Lógica de entrada e rotas
├── Model/                 → Definições de entidades (e.g., Post, Usuario)
├── Service/               → Regras de negócio
├── Validator/             → Validação de dados (ex: FluentValidation)
├── Data/                  → Acesso a dados (DbContext, repositórios)
├── Properties/            → Configurações do projeto
├── Program.cs             → Configuração principal e inicialização
├── appsettings.json       → Configuração geral
├── appsettings.Development.json → Configurações específicas para dev
├── blogpessoal.csproj     → Arquivo de projeto .NET
└── blogpessoal.sln        → Solution

Instalação & Execução
# Clonar o repositório
git clone https://github.com/geandrol/Blogpessoal-ASP.NET.git

# Acessar a pasta do projeto
cd Blogpessoal-ASP.NET

# Restaurar pacotes
dotnet restore

# Executar a aplicação
dotnet run

# Ou abrir no Visual Studio / VS Code e rodar em modo de depuração

Configuração

Atualize appsettings.json com as configurações do seu ambiente (conexão com banco, etc).

Utilize appsettings.Development.json para configurações de desenvolvimento local.

Exemplos de variáveis:

{
  "ConnectionStrings": {
    "DefaultConnection": "Server=.;Database=BlogPessoal;Trusted_Connection=True;"
  },
  "Logging": {
    "LogLevel": {
      "Default": "Information"
    }
  }
}

Boas Práticas

Mantenha controllers finos: utilize Services para manipular lógica.

Valide input no Validator antes de persistir dados.

Separe ambientes (Desenvolvimento, Produção) com arquivos de configuração diferentes.

Utilize injeção de dependência (DI) para instanciar Services, Validators, DbContext.

Contribuição

Contribuições são bem-vindas! Veja como ajudar:

Faça um fork deste repositório.

Crie uma branch com sua feature (git checkout -b feature/nova-feature).

Faça commit das suas alterações (git commit -m "Descrição da feature").

Envie ao repositório original (git push origin feature/nova-feature).

Abra um Pull Request para revisão.
