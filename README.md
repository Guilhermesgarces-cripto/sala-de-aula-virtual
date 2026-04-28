# 🎓 Sala de Aula Virtual - Comando ADS

**Um ambiente de estudos imersivo estilo "Terminal Hacker" projetado para estudantes de tecnologia.**

Este projeto é uma ferramenta de produtividade focada em imersão. Ao invés de pastas caóticas no computador ou blocos de notas espalhados, a Sala de Aula Virtual unifica anotações ricas, controle de tempo (Pomodoro) e persistência de dados no navegador através da API **IndexedDB**.

---

## ✨ Funcionalidades Principais

- ⏱️ **Timer Pomodoro Integrado**: Controle seu tempo de estudo e descanso (25min / 5min) diretamente no topo da tela, com feedback visual.
- 💾 **Persistência com IndexedDB**: Suas anotações, cursos e tópicos são salvos no banco de dados interno do seu navegador (`indexedDB`). Não há dependência de servidores, mantendo a ferramenta ultra-rápida e privada.
- 🎨 **Editor de Texto Rico (WYSIWYG)**: Permite formatar anotações técnicas, adicionar imagens, links e realçar sintaxes usando `execCommand`.
- 📁 **Organização Hierárquica**: Crie Módulos/Semestres, adicione Disciplinas dentro deles, e crie Tópicos específicos para cada aula.
- 👨‍💻 **Design "Dark Mode Premium"**: Interface com estética de terminal clássico, fonte `JetBrains Mono` e brilhos em neon vermelho.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 & CSS3** (Vanilla, CSS Variables, Flexbox, Grid)
- **JavaScript (ES6+)**
- **IndexedDB API** (Armazenamento Local Estruturado)
- **Phosphor Icons / Remix Icon** (Ícones da Interface)
- **Google Fonts** (`JetBrains Mono` e `Inter`)

---

## 🚀 Como Acessar

O projeto está hospedado no GitHub Pages e pode ser utilizado diretamente pelo navegador, sem necessidade de instalação:

🔗 **[Acessar o Sistema](https://guilhermesgarces-cripto.github.io/sala-de-aula-virtual/)**  
📊 **[Apresentação do Projeto](https://guilhermesgarces-cripto.github.io/sala-de-aula-virtual/apresentacao.html)**

---

## 💻 Como Rodar Localmente

Caso queira baixar e rodar o projeto localmente para fazer modificações:

1. Clone o repositório:
```bash
git clone https://github.com/Guilhermesgarces-cripto/sala-de-aula-virtual.git
```
2. Abra a pasta do projeto.
3. Como o projeto utiliza IndexedDB e módulos puramente no client-side, **recomenda-se abrir via Live Server** (extensão do VSCode) para evitar bloqueios de CORS do navegador em arquivos `file://`.
4. Abra o arquivo `index.html`.

---

## 🧠 Arquitetura de Armazenamento (IndexedDB)

O banco de dados `ADSDatabase` possui 3 "Object Stores" principais:
1. `courses` (Cursos/Semestres)
2. `subjects` (Matérias/Disciplinas - vinculadas aos Cursos)
3. `topics` (Tópicos/Anotações - vinculadas às Matérias)

Isso permite armazenar textos longos formatados em HTML sem os gargalos de tamanho do `localStorage`.

---

## 🧑‍💻 Autor

**Guilherme Garces**  
*Desenvolvedor Frontend*  
[Perfil no GitHub](https://github.com/Guilhermesgarces-cripto)
