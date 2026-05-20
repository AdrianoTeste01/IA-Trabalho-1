# 🚛 Logística Brasil — Trabalho de Inteligência Artificial

Sistema desenvolvido para a disciplina de Inteligência Artificial do IFSC — Campus Lages, utilizando algoritmos clássicos de grafos aplicados à logística brasileira.

---

# 📚 Sobre o Projeto

O projeto simula uma rede logística entre capitais brasileiras utilizando:

* 🚗 Transporte rodoviário
* 🚆 Transporte ferroviário
* 🧠 Algoritmos de Inteligência Artificial
* 📍 Busca heurística
* 🌐 Grafos
* 🧬 Algoritmos genéticos

A aplicação possui:

* Backend em Python com FastAPI
* Frontend em HTML, CSS e JavaScript
* Integração via API REST
* Interface interativa para visualização das rotas

---

# 🧠 Algoritmos Implementados

## ✅ A* (A-Estrela)

Responsável por encontrar o melhor caminho entre duas capitais considerando:

* distância total
* custo de transporte
* heurística baseada em coordenadas geográficas

### Custo utilizado

```text
R$ 5,00 por km
```

---

## ✅ Kruskal

Utilizado para gerar uma:

```text
Árvore Geradora Mínima
```

Representando uma malha ferroviária nacional com menor custo possível.

### Objetivo

Conectar todas as capitais com:

* menor distância total
* menor custo de implantação

### Custo utilizado

```text
R$ 2.000.000 por km
```

---

## ✅ A* com Ferrovia

Versão híbrida do algoritmo A* utilizando:

* rodovias
* malha ferroviária gerada pelo Kruskal

### Custos

| Tipo       | Valor      |
| ---------- | ---------- |
| Rodovia    | R$ 5,00/km |
| Ferrovia   | R$ 1,20/km |
| Transbordo | R$ 1.000   |

---

## ✅ Algoritmo Genético

Simula otimização de malha ferroviária utilizando:

* população
* mutação
* elitismo
* gerações

Objetivo:

```text
Encontrar soluções com menor custo logístico
```

---

# 🗺️ Estrutura do Grafo

O sistema utiliza:

* Capitais brasileiras
* Distâncias reais aproximadas
* Ligações entre estados vizinhos
* Coordenadas geográficas para heurística

---

# 🏗️ Estrutura do Projeto

```text
Trabalho IA - Ferrovias/
│
├── app.py
├── grafo_dados.py
├── index.html
├── requirements.txt
└── README.md
```

---

# ⚙️ Tecnologias Utilizadas

## Backend

* Python 3.12
* FastAPI
* Uvicorn

## Frontend

* HTML5
* CSS3
* JavaScript

---

# 🚀 Como Executar o Projeto

# 1️⃣ Clonar o repositório

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

---

# 2️⃣ Entrar na pasta

```bash
cd "Trabalho IA - Ferrovias"
```

---

# 3️⃣ Criar ambiente virtual

## Windows

```bash
python -m venv venv
```

---

# 4️⃣ Ativar ambiente virtual

## PowerShell

```bash
.\venv\Scripts\activate
```

---

# 5️⃣ Instalar dependências

```bash
pip install fastapi uvicorn
```

---

# 6️⃣ Executar API

```bash
python -m uvicorn app:app --reload
```

Servidor:

```text
http://127.0.0.1:8000
```

---

# 7️⃣ Abrir Frontend

Abra o arquivo:

```text
index.html
```

no navegador.

---

# 🔌 Rotas da API

## Página inicial

```http
GET /
```

---

## Algoritmo A*

```http
GET /a-estrela
```

### Parâmetros

| Nome    | Tipo   |
| ------- | ------ |
| origem  | string |
| destino | string |

### Exemplo

```http
/a-estrela?origem=Curitiba&destino=Salvador
```

---

## Algoritmo de Kruskal

```http
GET /kruskal
```

---

# 🎨 Interface

O sistema possui:

* Navegação por abas
* Visualização de rotas
* Exibição de custos
* Resultados detalhados
* Layout estilo GitHub Dark

---

# 📊 Funcionalidades

## ✔️ Cálculo de rotas

* distância total
* caminho percorrido
* custo logístico

## ✔️ Geração de malha ferroviária

* árvore mínima
* custo de implantação

## ✔️ Integração Frontend + Backend

* consumo de API REST
* atualização dinâmica da interface

---

# 📌 Conceitos Aplicados

* Grafos
* Heurística
* Busca A*
* Árvore Geradora Mínima
* Union-Find
* Algoritmos Genéticos
* APIs REST
* Estruturas de Dados

---

# 👨‍💻 Desenvolvido por

Adriano Ribeiro

IFSC — Instituto Federal de Santa Catarina
Campus Lages
Curso de Ciência da Computação

---

# 📖 Disciplina

Inteligência Artificial

---

# 🏁 Resultado

O projeto demonstra como algoritmos clássicos de IA podem ser utilizados para:

* otimização logística
* planejamento de transporte
* redução de custos
* modelagem de redes

aplicando conceitos reais de computação em um cenário inspirado na infraestrutura brasileira.
