# Aterma_civ_tjma
Uma aplicação web projetada para otimizar o processo de atermação — a redução a termo das reclamações cíveis — nos Juizados Especiais, potencializando o princípio do Jus Postulandi.

Acesse aqui a ferramenta (https://g.co/gemini/share/66aa63146935)

# Assistente de Atermação com IA ⚖️

Uma aplicação web projetada para otimizar o processo de **atermação** — a redução a termo das reclamações cíveis — nos Juizados Especiais, potencializando o princípio do *Jus Postulandi*.

---

### 🎯 O Problema: A Complexidade da Atermação

O *Jus Postulandi* garante ao cidadão o direito de iniciar um processo nos Juizados Especiais sem um advogado. No entanto, o primeiro passo, a **atermação**, representa um desafio significativo. O servidor do juizado precisa ouvir o relato, muitas vezes informal e emocional, do cidadão, analisar diversas provas (áudios, fotos, documentos) e traduzir tudo isso em uma petição inicial juridicamente coesa e bem estruturada. Esse processo manual é:

* **Trabalhoso e demorado:** Exige que o servidor atue como entrevistador, analista e redator simultaneamente.
* **Subjetivo:** A qualidade do termo final pode variar muito dependendo da experiência do servidor.
* **Ineficiente:** Cria um gargalo no atendimento, especialmente em juizados com alto volume de reclamações.

---

### 💡 A Solução: Um Assistente Inteligente para Atermação

Este projeto nasceu para solucionar exatamente esse gargalo. É uma ferramenta de **Computação Aplicada** que serve como um assistente para o servidor do juizado, automatizando as partes mais trabalhosas do processo de atermação.

A aplicação guia o servidor através de um fluxo de trabalho passo a passo, utilizando Inteligência Artificial para:

1.  **Consolidar as Provas:** O servidor faz o upload de todos os arquivos fornecidos pelo cidadão (áudios, imagens, PDFs, etc.).
2.  **Gerar o Relato dos Fatos:** A IA analisa o conteúdo de todos os arquivos e gera uma narrativa cronológica e objetiva dos fatos, servindo como a base da reclamação.
3.  **Permitir a Revisão Humana:** O servidor pode revisar, editar e complementar o relato gerado pela IA, garantindo a precisão das informações.
4.  **Estruturar a Petição:** Com o relato finalizado, a IA utiliza um modelo de petição para montar a minuta completa da reclamação, preenchendo os fatos, qualificando as partes (com base nas informações) e estruturando os pedidos.
5.  **Entregar a Minuta Final:** A ferramenta entrega um documento formatado, pronto para ser revisado uma última vez e protocolado no sistema PJE.

---

### ✨ Arquitetura e Funcionalidades

Este projeto foi desenvolvido como uma aplicação de página única (SPA) com uma arquitetura de etapas (stepper), tornando a experiência do usuário clara e intuitiva.

* **Interface por Etapas:** O progresso visual (`Upload` -> `Revisão do Relato` -> `Modelo da Petição` -> `Minuta Final`) organiza o processo de atermação.
* **Processamento Multimodal (Simulado):** A capacidade de receber múltiplos tipos de arquivos demonstra como a IA pode centralizar e entender informações de diversas fontes.
* **Fluxo de Geração em Dois Passos com IA:**
    1.  **IA como Analista:** Primeiro, o Gemini atua como um assistente que ouve o caso e sintetiza os fatos.
    2.  **IA como Redator Jurídico:** Depois, o Gemini assume o papel de redator, pegando os fatos já validados e aplicando a estrutura formal de uma petição.
* **Componentização:** A aplicação utiliza componentes reutilizáveis (`HeaderStepper`, `LoadingSpinner`), seguindo as melhores práticas de desenvolvimento de software moderno.

---

### 🚀 Tecnologias e Plataformas

* **Framework:** React com Vite
* **Linguagem:** JavaScript (JSX)
* **Estilização:** Tailwind CSS e ícones `lucide-react`.
* **Inteligência Artificial:** Integração com a API do **Google Gemini** para as tarefas de análise e geração de texto.

