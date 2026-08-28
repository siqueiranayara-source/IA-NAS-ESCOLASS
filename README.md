# 🤖 IA nas Escolas - Analisador de Sentimentos

Bem-vindo ao projeto **Analisador de Sentimentos com IA**! Este é um projeto educacional desenvolvido para ensinar **Inteligência Artificial** nas escolas usando Python.

## 📚 O que é este projeto?

Este projeto utiliza **TextBlob** (uma biblioteca de Processamento de Linguagem Natural) para analisar o sentimento de frases em português. A interface foi criada com **Gradio**, tornando fácil para qualquer pessoa (sem conhecimento técnico) testar a IA!

## ✨ Recursos

- ✅ Análise de sentimentos em tempo real
- ✅ Interface web intuitiva e bonita
- ✅ Classificação em 3 categorias: Positivo, Negativo, Neutro
- ✅ Nota de polaridade (-1 a +1)
- ✅ Exemplos pré-carregados
- ✅ Perfeito para aulas de IA

## 🎯 Como Usar

### 1️⃣ Instalação

Primeiro, certifique-se de ter Python 3.7+ instalado.

Clone o repositório:
```bash
git clone https://github.com/siqueiranayara-source/IA-NAS-ESCOLASS.git
cd IA-NAS-ESCOLASS
```

Instale as dependências:
```bash
pip install -r requirements.txt
```

### 2️⃣ Executar o Projeto

```bash
python analisador_sentimentos.py
```

Você verá uma saída como:
```
Running on local URL:  http://127.0.0.1:7860
```

Abra este link no seu navegador! 🌐

### 3️⃣ Usar a Interface

1. Digite uma frase na caixa de texto
2. Clique em "Submit"
3. Veja o resultado: 😊 Positivo, 😞 Negativo ou 😐 Neutro

## 🔍 Exemplos

| Frase | Resultado |
|-------|-----------|
| "Estou muito feliz hoje!" | 😊 POSITIVO (nota: 0.70) |
| "Hoje foi um dia péssimo." | 😞 NEGATIVO (nota: -0.80) |
| "O tempo está nublado." | 😐 NEUTRO (nota: 0.00) |

## 🧠 Como Funciona?

### TextBlob
TextBlob analisa o texto e calcula uma **polaridade** (sentimento):
- `> 0.1` = Sentimento POSITIVO ✅
- `< -0.1` = Sentimento NEGATIVO ❌
- `-0.1 a 0.1` = Sentimento NEUTRO ⚪

### Gradio
Gradio cria uma interface web automática para seu código Python, sem precisar conhecer HTML/CSS/JavaScript!

## 📁 Estrutura do Projeto

```
IA-NAS-ESCOLASS/
├── analisador_sentimentos.py    # Código principal
├── requirements.txt              # Dependências
└── README.md                      # Este arquivo
```

## 🎓 Aprendizados

Com este projeto, você aprenderá:
- ✅ Processamento de Linguagem Natural (NLP)
- ✅ Como usar bibliotecas de IA
- ✅ Criar interfaces gráficas com Gradio
- ✅ Análise de sentimentos
- ✅ Git e GitHub

## 🚀 Próximos Passos

Quer melhorar o projeto? Tente:
- 🎨 Adicionar mais exemplos
- 📊 Criar um gráfico com histórico de análises
- 🌐 Suportar outros idiomas
- 💾 Salvar resultados em um arquivo
- 🔗 Deploy na nuvem (Hugging Face Spaces, Gradio Hosting)

## 📝 Licença

Este projeto é de código aberto e livre para usar na educação!

## 👨‍🏫 Autor

Desenvolvido por **Nayara Siqueira** para fins educacionais.

---

**Aprenda IA de forma divertida! 🤖✨**
