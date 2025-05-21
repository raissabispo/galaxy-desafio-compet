
# 🔭 Classificação de Galáxias com Inteligência Artificial

Este projeto utiliza um modelo de machine learning treinado para classificar galáxias com base em probabilidades fornecidas para três categorias: **elíptica**, **espiral** e **não galáxia**. A interface foi desenvolvida com [Gradio](https://www.gradio.app/) para permitir que qualquer pessoa interaja facilmente com o modelo.

---

## 🚀 Tecnologias Utilizadas

- Python 3.10+
- Pandas
- Pickle
- Gradio
- Scikit-learn (para o treinamento do modelo)

---

## 📁 Estrutura do Projeto

```

├── melhor\_modelo.pkl        # Modelo treinado serializado com Pickle
├── app.py                   # Código principal com a interface Gradio
├── README.md                # Documentação do projeto

````

---

## 🎯 Objetivo

Permitir a previsão do tipo de galáxia com base em probabilidades fornecidas manualmente. O modelo foi treinado a partir de dados do projeto Galaxy Zoo.

---

## 💻 Como Executar Localmente

1. Clone o repositório:

```bash
git clone https://github.com/raissabispo/galaxy-desafio-compet.git
cd seu-repositorio
````

2. Crie um ambiente virtual (opcional, mas recomendado):

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Execute a aplicação:

```bash
python app.py
```

A aplicação será aberta automaticamente no navegador com a interface do Gradio.

---

## 📌 Como Funciona

O usuário deve inserir três probabilidades, cujos valores devem estar entre **0 e 1**:

* `espiral` → Probabilidade da galáxia ser do tipo espiral
* `eliptica` → Probabilidade da galáxia ser do tipo elíptica
* `nao_galaxia` → Probabilidade de não ser uma galáxia ou ser de outro tipo

> **Importante:** A **soma dos três valores deve estar entre 0.95 e 1.05**, pois eles representam probabilidades.

---

## ✅ Exemplo de Entrada e Saída

| Elíptica | Espiral | Não Galáxia | Saída Esperada               |
| -------- | ------- | ----------- | ---------------------------- |
| 0.6      | 0.3     | 0.1         | Classe prevista: elíptica    |
| 0.1      | 0.8     | 0.1         | Classe prevista: espiral     |
| 0.2      | 0.3     | 0.5         | Classe prevista: não galáxia |

---

## 💬 Explicação Simples

O modelo recebeu dados históricos sobre galáxias e aprendeu a identificar padrões. Quando você fornece os valores (ex: 0.7 para espiral, 0.2 para elíptica e 0.1 para não galáxia), ele utiliza esse conhecimento para prever qual tipo de galáxia mais se encaixa nessa combinação.

---

## ✨ Interface

A interface é feita com Gradio, e é muito fácil de usar:

* Campos de entrada para as 3 probabilidades
* Mensagens de erro amigáveis
* Retorno textual com a **classe prevista**

---

## 👩‍💻 Desenvolvido por

**Raissa Vitória**
Estudante de Análise e Desenvolvimento de Sistemas
Apaixonada por tecnologia, QA e inteligência artificial

---

## 📜 Licença

Este projeto é de livre uso acadêmico e educacional. Sinta-se à vontade para adaptar ou expandir.


```
