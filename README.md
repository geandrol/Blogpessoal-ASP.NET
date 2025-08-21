# 📖 BlogPessoal - ASP.NET Core

Projeto desenvolvido em **ASP.NET Core** para criação de um **Blog Pessoal**, aplicando boas práticas de arquitetura em camadas, validação, serviços e organização de código.  

---

## 🚀 Sobre o Projeto

O **BlogPessoal** é uma aplicação web que serve como base para estudo e implementação de um blog.  
A ideia principal é estruturar um backend robusto que pode ser consumido por diferentes frontends (React, Angular, Vue ou até mobile).  

---

## ✨ Funcionalidades

- 📌 CRUD de postagens e temas  
- 🗂️ Organização em camadas (Controllers, Models, Services, Validators)  
- ✅ Validação de dados para maior consistência  
- ⚙️ Configuração separada por ambiente (`Development` e `Production`)  
- 🔒 Pronto para expansão com autenticação e autorização  
- 🛠️ Fácil manutenção e escalabilidade  

---

## 🛠️ Tecnologias Utilizadas

- [.NET](https://dotnet.microsoft.com/) (ex.: .NET 7 ou 8)  
- [ASP.NET Core](https://learn.microsoft.com/aspnet/core)  
- [C#](https://learn.microsoft.com/dotnet/csharp/)  
- Entity Framework Core *(se aplicável)*  
- FluentValidation *(se aplicável)*  

---

## 📂 Estrutura do Projeto

```bash
/BlogPessoal-ASP.NET
│
├── Controller/             # Camada de controle e rotas da API
├── Model/                  # Modelos/entidades do sistema
├── Service/                # Regras de negócio
├── Validator/              # Validação de dados
├── Data/                   # Acesso a banco de dados (DbContext)
├── Properties/             # Configurações do projeto
├── Program.cs              # Arquivo principal de inicialização
├── appsettings.json        # Configuração geral
├── appsettings.Development.json  # Configurações específicas do ambiente Dev
├── blogpessoal.csproj      # Arquivo de configuração do projeto
└── blogpessoal.sln         # Solution .NET
```

---

## ⚡ Como Executar o Projeto

### Pré-requisitos
- [.NET SDK](https://dotnet.microsoft.com/download) instalado  
- Banco de dados configurado (se aplicável)  
- Visual Studio / VS Code  

### Passos

```bash
# Clonar o repositório
git clone https://github.com/geandrol/Blogpessoal-ASP.NET.git

# Acessar a pasta
cd Blogpessoal-ASP.NET

# Restaurar pacotes
dotnet restore

# Executar a aplicação
dotnet run
```

A API estará disponível em:  
👉 `https://localhost:5001` (HTTPS)  
👉 `http://localhost:5000` (HTTP)  

---

## ⚙️ Configuração

Edite o arquivo `appsettings.json` para ajustar conexões e logs:  

```json
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
```

---

## 🤝 Contribuindo

1. Faça um **fork** do projeto  
2. Crie uma **branch** para sua feature (`git checkout -b feature/minha-feature`)  
3. Faça **commit** das suas mudanças (`git commit -m 'Minha nova feature'`)  
4. Envie para o repositório (`git push origin feature/minha-feature`)  
5. Abra um **Pull Request** 🚀  

---

## 📜 Licença

Este projeto está sob a licença **MIT**.  
Sinta-se livre para usar, modificar e compartilhar.  

---

👨‍💻 Desenvolvido por **[Geandro Araujo](https://github.com/geandrol)**  
