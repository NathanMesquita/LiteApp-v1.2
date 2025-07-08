# 📇 LiteApp v1.2

**LiteApp** é um aplicativo leve e intuitivo para cadastro e gerenciamento de contatos, desenvolvido em **C# com Windows Forms**.  
Ideal para iniciantes que estão aprendendo sobre desenvolvimento de aplicações desktop com persistência de dados.

> 🎉 Esta versão 1.2 traz a funcionalidade de **exclusão de contatos** da lista.

---

## 🚀 Funcionalidades da versão 1.2

- ✅ Interface gráfica simples e fácil de usar (WinForms)
- ✅ Cadastro de contatos com **Nome** e **Telefone**
- ✅ **Salvamento automático** dos contatos em um arquivo `.json`
- ✅ Carregamento automático dos contatos ao abrir o app
- ✅ Botão **"Limpar"** para resetar os campos
- ✅ **Botão "Excluir"** para remover contatos selecionados
- ✅ Dados persistentes (não somem ao fechar o app)

---

## 🧱 Estrutura da solução

LiteAppSolution/
├── LiteApp.Domain/ # Modelo de dados (Contato.cs)
├── LiteApp.Data/ # Repositório e persistência JSON (ContatoRepository.cs)
├── LiteApp.UI/ # Interface com Windows Forms (Form1.cs)
└── contatos.json # Arquivo com os contatos salvos

---

## 📸 Interface

A interface contém:

- Campos de entrada para **Nome** e **Telefone**
- Botões: `Adicionar`, `Limpar` e `Excluir`
- Lista de contatos (ListBox) com os registros

> Contatos são exibidos no formato:  
> `João da Silva - (11) 99999-9999`

---

## 💾 Como funciona o salvamento

- O arquivo `contatos.json` é criado automaticamente
- Toda modificação (adição ou exclusão) atualiza o conteúdo do arquivo
- Ao iniciar o aplicativo, os dados são carregados automaticamente

---

## 🛠️ Tecnologias utilizadas

- 🧩 C#
- 🖼️ Windows Forms (.NET Framework)
- 📦 Newtonsoft.Json (via NuGet)

---

## ▶️ Como executar

1. Abra a solução `LiteAppSolution.sln` no Visual Studio
2. Compile com `Ctrl + Shift + B`
3. Execute o projeto `LiteApp.UI`
4. Adicione, exclua e visualize seus contatos com persistência local

---

## 📌 Melhorias previstas (versão 1.3+)

- [ ] Edição de contatos
- [ ] Busca por nome/telefone
- [ ] Exportar lista para `.csv`
- [ ] Organização por ordem alfabética
- [ ] Criar instalador `.exe`

---

## 👤 Autor

Desenvolvido por [NathanMesquita]  
Projeto criado com fins didáticos para prática de C# e Windows Forms.
