# AgroCitro

AgroCitro é um sistema web desenvolvido para gerenciar informações de uma fazenda de laranjas, integrando banco de dados com a interface web. O sistema contempla registros de **colheita**, **irrigação** e **plantio**, permitindo que os gestores da fazenda acompanhem todas as etapas da produção de forma organizada.

---

## 📌 Grupo Desenvolvedor

- **Guilherme Oliveira Lisboa**  
- **Tiago Padovani Cardoso**  
- **Ana Julia Costilho Martins**  
- **Lucas Grosa Takano**  

---

## 🛠️ Tecnologias Utilizadas

- **HTML**: Estrutura da interface web  
- **CSS**: Estilização do site, tornando a interface agradável e intuitiva  
- **JavaScript**: Funcionalidades interativas, validação de formulários e manipulação dinâmica de dados  
- **Banco de Dados**: Sistema relacional (ex: MySQL ou PostgreSQL) para armazenamento das informações de colheita, irrigação e plantio  

---

## 🗂️ Estrutura do Banco de Dados

O banco de dados do AgroCitro possui três tabelas principais:

1. **Plantio**
   - `id_plantio` (PK)
   - `tipo_laranja`
   - `data_plantio`
   - `quantidade_plantada`
   - `localizacao`

2. **Irrigação**
   - `id_irrigacao` (PK)
   - `id_plantio` (FK)
   - `data_irrigacao`
   - `quantidade_agua`
   - `responsavel`

3. **Colheita**
   - `id_colheita` (PK)
   - `id_plantio` (FK)
   - `data_colheita`
   - `quantidade_colhida`
   - `qualidade`

---

## 🖥️ Estrutura do Site

### HTML
- Criação de páginas para cada módulo (Plantio, Irrigação, Colheita)  
- Formulários para inserir, editar e excluir dados  
- Tabelas para visualizar os registros

### CSS
- Layout responsivo para desktop e mobile  
- Paleta de cores inspirada na natureza (tons de laranja e verde)  
- Destaque visual para informações importantes, como alertas de irrigação ou colheita

### JavaScript
- Validação de formulários antes do envio para o banco de dados  
- Atualização dinâmica de tabelas sem recarregar a página (AJAX ou Fetch API)  
- Mensagens de sucesso e erro em operações de CRUD (Create, Read, Update, Delete)

---

## ⚙️ Funcionalidades do Sistema

1. **Plantio**
   - Cadastro de novos plantios  
   - Registro de detalhes da plantação, quantidade e localização  

2. **Irrigação**
   - Registro de irrigação diária ou programada  
   - Associação de cada irrigação ao plantio correspondente  

3. **Colheita**
   - Registro de colheita por data e plantio  
   - Avaliação da quantidade e qualidade da colheita  

4. **Visualização de Dados**
   - Consulta de histórico de plantio, irrigação e colheita  
   - Relatórios resumidos para facilitar o gerenciamento  

---

