# 📱 Lista de Tarefas - CodeStudio

![Versão](https://img.shields.io/badge/versão-1.0-blue)
![CodeStudio](https://img.shields.io/badge/CodeStudio-Compatible-green)
![Android](https://img.shields.io/badge/Android-7.0+-brightgreen)
![Licença](https://img.shields.io/badge/licença-MIT-orange)

## Sobre o Projeto

**Lista de Tarefas** é um aplicativo de gerenciamento de tarefas diárias que permite ao usuário criar, editar, excluir e visualizar suas tarefas de forma organizada. Cada tarefa possui título, descrição e data/hora de criação.

O app foi desenvolvido inteiramente no **CodeStudio**, IDE mobile nativa para Android. Todo o código-fonte, layout, lógica de banco de dados e assinatura do APK foram executados no celular. Java puro, SQLite local, sem AndroidX.

### Funcionalidades do App

- ➕ Adicionar nova tarefa
- ✏️ Editar tarefa existente
- 🗑️ Excluir tarefa
- ⚡ Clique longo para ações rápidas (duplicar, copiar título, excluir rápido)
- 📅 Data e hora automática da criação
- 🎨 Interface com cards e design moderno

### Capturas de Tela

| Tela Principal | Adicionar Tarefa | Menu Rápido |
|----------------|------------------|-------------|
| `[screenshot1]` | `[screenshot2]` | `[screenshot3]` |

## ⚠️ Por que este projeto é "complexo" para o CodeStudio?

Diferente de apps simples de uma tela, este projeto demonstra:

| Desafio | Como o CodeStudio resolve |
|---------|---------------------------|
| Múltiplas Activities | Navegação entre telas com `Intent` |
| Banco de dados SQLite | `SQLiteOpenHelper` com CRUD completo |
| Adapter personalizado | `BaseAdapter` para exibir dados no ListView |
| Layouts aninhados | Cards dentro de RelativeLayout/FrameLayout |
| Drawables customizados | Botões, FAB, inputs com estilos próprios |
| Cliques longo e curto | Dois listeners diferentes no mesmo componente |

Este projeto prova que o CodeStudio aguenta apps com arquitetura real, não apenas "hello world".

## 📁 Estrutura do Projeto

```

ListaTarefas/
├── app/
│   ├── src/main/java/com/listatarefas/
│   │   ├── MainActivity.java          # Tela principal com lista
│   │   ├── AddTarefaActivity.java     # Tela de adicionar/editar
│   │   ├── DatabaseHelper.java        # Banco de dados SQLite
│   │   ├── Tarefa.java                # Modelo da tarefa
│   │   └── TarefaAdapter.java         # Adaptador para a lista
│   └── src/main/res/
│       ├── drawable/                   # Botões, FAB, inputs, cards
│       ├── layout/                     # activity_main, activity_add, item_tarefa
│       └── values/                     # colors, strings, styles

```

## 📦 Como compilar no CodeStudio

1. Baixe o ZIP deste repositório (botão verde "Code" → "Download ZIP")
2. Descompacte a pasta
3. Mova a pasta para o diretório de projetos do CodeStudio
4. Abra o CodeStudio e importe o projeto
5. Clique em **RUN**

> ✅ O APK será compilado e assinado diretamente no seu celular.

## 🐛 Erros?

Se encontrar algum erro durante a compilação, abra uma **Issue** aqui no GitHub com a mensagem de erro completa.

## 📄 Licença

**MIT License** - Você é livre para:
- Usar este código em qualquer projeto (pessoal ou comercial)
- Modificar, copiar, distribuir
- Subir como seu próprio app

Não é necessário dar créditos, mas é bem-vindo.

## 👨‍💻 Desenvolvedor

**TCLabs** - Cabinda, Angola

---

**Feito no CodeStudio. Compilado no celular. Livre para copiar.**
