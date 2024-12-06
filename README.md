# Painéis Gerenciais

Este projeto é uma aplicação web interativa para visualização e análise de painéis gerenciais. Ele oferece uma visão detalhada de diferentes aspectos operacionais, como receita por município, capacidade de distribuição e atendimento, e maximização de recursos. Você pode personalizar completamente o projeto, alterando links, cores, imagens e outros elementos diretamente no arquivo HTML, permitindo que ele atenda às suas necessidades específicas.

## 📂 Estrutura do Projeto

A organização dos arquivos no projeto é a seguinte:

```
MeuProjeto/
├── index.html         # Página principal com os painéis
├── mapa_.html         # Página com informações georreferenciadas
├── assets/
│   ├── images/
│   │   ├── 01_image.png
│   │   ├── Atendimento.png
│   │   ├── Capa.png
│   │   ├── Distribuição.png
│   │   ├── Munic_image.png
│   │   ├── max_.png
│   ├── css/
│   │   ├── styles.css (opcional: estilos externos)
│   ├── js/
│       ├── script.js (opcional: scripts externos)
├── data/
│   ├── noticias.json  # Arquivo JSON com dados de notícias
├── README.md          # Arquivo com instruções do projeto
```

## 🖥️ Funcionalidades

- **Receita por Município**: Painel que apresenta a receita operacional total segmentada por região, estados e municípios.
- **Receita Diária**: Painel detalhando a performance operacional diária planejada e executada.
- **Capacidade de Atendimento**: Painel que analisa processos de atendimento, margem de contribuição e utilização de canais.
- **Capacidade de Distribuição**: Painel com insights sobre eficiência na distribuição de recursos e carga de trabalho.
- **Maximização de Recursos**: Painel que detalha as despesas e analisa a proximidade geográfica e indicadores de desempenho.

## 🌟 Como Usar

1. Clone o repositório para sua máquina:
   ```bash
   git clone https://github.com/seuusuario/seurepositorio.git
   ```
2. Abra o arquivo `index.html` no navegador para acessar o projeto.

## 📜 Pré-requisitos

- Navegador atualizado (Google Chrome, Mozilla Firefox, Edge, etc.).
- Conexão com a internet para acessar os links externos e fontes.

## 📊 Exemplos de Painéis

- **Receita por Município**:  
  ![Exemplo de Receita por Município](assets/images/Munic_image.png)

- **Maximização de Recursos**:  
  ![Exemplo de Maximização de Recursos](assets/images/max_.png)

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estruturação do conteúdo.
- **CSS3**: Estilização visual.
- **JavaScript**: Funcionalidades dinâmicas.
- **Font Awesome**: Ícones para melhor apresentação.
- **Power BI**: Painéis interativos integrados via links externos.

### Como Personalizar os Links no HTML


Você pode facilmente editar e incluir novos links no projeto diretamente no arquivo HTML. Siga estas etapas:


#### **1. Estrutura Básica de um Link no HTML**
No arquivo `HTML`, os links estão definidos usando a tag `<a>`. A estrutura básica é a seguinte:

```html
<a href="SEU_LINK_AQUI" target="_blank">
    <i class="CLASSE_DO_ÍCONE"></i> Texto ou descrição do link
</a>
```

- **`href`**: Define o endereço do link. Substitua `SEU_LINK_AQUI` pelo URL desejado.
- **`target="_blank"`**: Faz com que o link abra em uma nova aba.
- **`<i>`**: Adiciona um ícone ao lado do texto (opcional, usa Font Awesome).
- **Texto ou descrição do link**: O texto visível para o usuário.



#### **2. Exemplo de Links no Projeto**

Os links existentes estão organizados assim:

```html
<a onclick="carregarPagina('metodologias.html')">
    <i class="fas fa-file-invoice-dollar"></i> Informações de Receita
</a>

<a href="mapa_.html" target="_blank">
    <i class="fas fa-map-marker-alt"></i> Metodologias de Custeio
</a>
```

- Para editar o **primeiro link**: Altere o arquivo que será carregado (`metodologias.html`).
- Para editar o **segundo link**: Substitua `mapa_.html` pelo endereço ou página desejada.

---

#### **3. Adicionar um Novo Link**

1. **Escolha o local no HTML onde deseja adicionar o link** (dentro do menu lateral ou em outra seção).
2. Copie e cole este exemplo de estrutura:

```html
<a href="SEU_NOVO_LINK.html" target="_blank">
    <i class="fas fa-link"></i> Seu Novo Link
</a>
```

3. Substitua:
   - **`SEU_NOVO_LINK.html`** pelo endereço do link ou página.
   - **`fa-link`** pela classe do ícone que deseja usar. Consulte os ícones disponíveis no [Font Awesome](https://fontawesome.com/icons).
   - **`Seu Novo Link`** pelo texto que descreve o link.

---

#### **4. Alterar um Link Existente**

Para alterar um link já presente no HTML:
1. Localize o trecho correspondente ao link que deseja editar.
2. Modifique o atributo `href` com o novo endereço.

**Exemplo:**
Antes:
```html
<a href="https://www.ibge.gov.br/indicadores.html" target="_blank">
    <i class="fas fa-chart-line"></i> Indicadores
</a>
```

Depois:
```html
<a href="https://exemplo.com/novo-indicador" target="_blank">
    <i class="fas fa-chart-line"></i> Novo Indicador
</a>
```

---

#### **5. Alterar Cores e Estilos dos Links**

As cores e estilos dos links são definidos no CSS. Você pode ajustá-los alterando a classe ou adicionando um estilo inline:

**Alterar cor apenas para um link específico:**
```html
<a href="SEU_LINK_AQUI" style="color: red;">
    <i class="fas fa-info-circle"></i> Link Vermelho
</a>
```

---

#### **6. Testar as Alterações**

Após editar o HTML:
1. Salve o arquivo.
2. Abra o `index.html` em um navegador para testar os novos links.






Desenvolvido por [Eric Vieira]. 🚀
