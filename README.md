# Projeto WordPress - Revenda de Veículos Elétricos

## Visão Geral
Este projeto consiste na criação de um site para uma revenda de veículos elétricos, desenvolvido em WordPress. O projeto incluirá um **tema customizado** e um **plugin** para gerenciamento de veículos. Desenvolvedores juniores irão implementá-lo com a orientação de um mentor.

---

## 📌 Estrutura de Páginas

### 1. Página Inicial
- Sessão de **banner**
- **Filtro de veículos** (widget reutilizável)
- **Veículos em destaque da semana** (widget)
- Últimas notícias (dados externos)

### 2. Página de Estoque
- **Listagem de veículos**
- **Filtro avançado** (widget reutilizável)

### 3. Página de Detalhes do Veículo
- Exibição de **todas as informações do veículo**
- Galeria de imagens
- **Veículos similares** (widget reutilizável)

### 4. Página de Notícias
- Carregamento de notícias **via API externa**

### 5. Página Sobre
- Informações institucionais

### 6. Página de Contato
- Formulário de contato
- Informações da loja

---

## 🧩 Widgets
Para maior flexibilidade, a maioria dos componentes serão widgets configuráveis pelo administrador.

### Principais Widgets:
- **Filtro de veículos**
- **Veículos em destaque**
- **Veículos similares**
- **Últimas notícias**
- **Banner promocional**

Cada widget terá opções de configuração via Admin para personalização total.

---

## 🔗 API de Integração
Os veículos serão cadastrados **via API externa**. Além disso, o Admin terá uma opção para **importar veículos manualmente** em formato **JSON** ou **XML**.

### Como a API funcionará:
1. Criar um **endpoint** para importar veículos
2. Criar um **cron job** para rodar a importação periodicamente

Exemplo de estrutura da API:
```json
{
  "marca": "Tesla",
  "modelo": "Model S",
  "ano": 2023,
  "preco": 350000,
  "imagem": "https://exemplo.com/model-s.jpg",
  "descricao": "Carro elétrico de luxo com autonomia de 600 km."
}
```

---

## ⚙️ Configurações no Admin
O painel administrativo permitirá:
- **Gerenciar veículos manualmente**
- **Configurar widgets**
- **Importar veículos (JSON/XML)**
- **Personalizar layout, cores e ordenação dos veículos**

---

## 🎨 Tema
- O tema será **desenvolvido do zero**
- Utilizará **Tailwind CSS** para estilização

---

## 🚀 Passo a Passo para os Desenvolvedores

1️⃣ Criar a estrutura base do **tema** (Pastas: `header.php`, `footer.php`, `index.php`, `functions.php`)
2️⃣ Criar o **plugin** para gerenciamento de veículos
3️⃣ Implementar os **widgets reutilizáveis**
4️⃣ Desenvolver a **API de integração**
5️⃣ Criar o **cron job** para atualizar os veículos automaticamente
6️⃣ Configurar as **opções do Admin** para personalização
7️⃣ Testar tudo e realizar ajustes

---

## 🛠 Tecnologias Utilizadas
- **WordPress** (Tema + Plugin)
- **Tailwind CSS** (Estilização)
- **PHP** (Back-end do WordPress)
- **REST API** (Integração de veículos)
- **Cron Jobs** (Importação automática)

---

## 📢 Conclusão
Esse projeto foi pensado para que desenvolvedores da Squad 3 possam praticar WordPress de forma orientada, criando uma solução real e totalmente customizável. Qualquer dúvida, consulte a documentação ou pergunte ao autor! 🚀
