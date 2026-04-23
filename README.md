# Calculadora de Emissão de CO₂ 🌿

[🌐 Acesse a aplicação aqui](https://karinabarros.github.io/calculadora-co2/)

Uma aplicação web interativa para calcular emissões de dióxido de carbono (CO₂) geradas por viagens entre cidades brasileiras, promovendo conscientização ambiental e sustentabilidade.

## 📋 Descrição

Esta calculadora permite aos usuários estimar o impacto ambiental de suas viagens, comparando diferentes meios de transporte e fornecendo informações sobre créditos de carbono necessários para compensar as emissões. Desenvolvida como projeto educacional para demonstrar conceitos de sustentabilidade e desenvolvimento web moderno.

## ✨ Funcionalidades

- **Cálculo de Emissões**: Estima emissões de CO₂ baseadas na distância e meio de transporte
- **Banco de Dados de Rotas**: Contém distâncias entre mais de 30 cidades brasileiras
- **Comparação de Transportes**: Mostra emissões relativas para bicicleta, carro, ônibus e caminhão
- **Sugestões de Cidades**: Autocomplete inteligente com datalist HTML5
- **Distância Manual**: Opção para inserir distâncias personalizadas
- **Créditos de Carbono**: Calcula quantidade necessária e estimativa de custo
- **Interface Responsiva**: Design adaptável para dispositivos móveis e desktop
- **Experiência do Usuário**: Estados de carregamento, validação de formulários e feedback visual

## 🛠️ Tecnologias Utilizadas

### Frontend
- **HTML5**: Estrutura semântica e acessível
- **CSS3**: Estilos responsivos com variáveis CSS e Flexbox/Grid
- **JavaScript (ES6+)**: Lógica de negócio e manipulação DOM

### Ferramentas de Desenvolvimento
- **Git**: Controle de versão
- **GitHub Pages**: Hospedagem gratuita
- **GitHub Actions**: CI/CD para deploy automático

## 🏗️ Arquitetura e Boas Práticas

### Princípios de Arquitetura
- **Separação de Responsabilidades**: Código organizado em módulos independentes
- **Modularidade**: Cada arquivo JS tem uma responsabilidade específica
- **Configuração Centralizada**: Constantes e fatores em arquivo dedicado
- **Reutilização de Código**: Funções utilitárias compartilhadas
- **Manutenibilidade**: Código comentado e bem estruturado

### Estrutura Arquitetural

```
📁 CalculadoraCO2/
├── 📄 index.html          # Estrutura HTML principal
├── 📁 css/
│   └── 📄 style.css       # Estilos visuais
└── 📁 js/
    ├── 📄 app.js         # Inicialização e controle principal
    ├── 📄 calculator.js  # Lógica de cálculos
    ├── 📄 config.js      # Configurações e constantes
    ├── 📄 routes-data.js # Banco de dados de rotas
    └── 📄 ui.js          # Renderização e manipulação DOM
```

### Padrões Implementados

#### 1. **Padrão de Módulos**
- Objetos globais (`Calculator`, `UI`, `CONFIG`, `RoutesDB`) encapsulam funcionalidades
- Métodos públicos expostos, detalhes de implementação ocultos

#### 2. **Separação de Camadas**
- **Apresentação (UI)**: Renderização e interações do usuário
- **Lógica de Negócio (Calculator)**: Cálculos e regras de negócio
- **Dados (RoutesDB)**: Acesso e manipulação de dados
- **Configuração (CONFIG)**: Constantes e configurações do sistema

#### 3. **Tratamento de Erros**
- Validação de entrada no frontend
- Try-catch em operações críticas
- Feedback amigável ao usuário

#### 4. **Performance**
- Cálculos otimizados
- Renderização eficiente do DOM
- Simulação de carregamento para UX

#### 5. **Acessibilidade**
- HTML semântico
- Labels adequados
- Navegação por teclado
- Contraste de cores

## 📁 Estrutura de Arquivos Detalhada

### `index.html`
- Estrutura HTML5 semântica
- Formulário com validação
- Seções para resultados dinâmicos
- Inclusão ordenada de scripts

### `css/style.css`
- Variáveis CSS para temas
- Layout responsivo com Grid e Flexbox
- Animações suaves
- Design system consistente

### `js/app.js`
- **Responsabilidade**: Inicialização e coordenação
- Event listeners para formulário
- Controle do fluxo de cálculo
- Tratamento de estados da aplicação

### `js/calculator.js`
- **Responsabilidade**: Lógica matemática
- Cálculos de emissões por modo de transporte
- Comparações e percentuais
- Estimativas de créditos de carbono

### `js/config.js`
- **Responsabilidade**: Configurações globais
- Fatores de emissão por transporte
- Metadados de modos de transporte
- Configurações de créditos de carbono
- Utilitários de interface (datalist, autofill)

### `js/routes-data.js`
- **Responsabilidade**: Dados de rotas
- Banco de dados de distâncias entre cidades
- Métodos de busca e filtragem
- Estrutura otimizada para consultas

### `js/ui.js`
- **Responsabilidade**: Interface do usuário
- Funções de formatação (números, moeda)
- Renderização de componentes HTML
- Manipulação de estados visuais (show/hide, loading)

## 🚀 Como Executar

### Pré-requisitos
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexão com internet (opcional, para deploy)

### Execução Local
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/calculadora-co2.git
   cd calculadora-co2
   ```

2. Abra o arquivo `index.html` no navegador:
   ```bash
   # No Windows
   start index.html
   
   # Ou simplesmente arraste o arquivo para o navegador
   ```

### Deploy no GitHub Pages
O projeto inclui configuração automática de deploy:
- Push para branch `main` dispara deploy
- URL: `https://seu-usuario.github.io/calculadora-co2`

## 💻 Desenvolvimento

### Configuração do Ambiente
1. Instale um editor de código (VS Code recomendado)
2. Configure live server para desenvolvimento local
3. Use ferramentas de desenvolvedor do navegador para debug

### Convenções de Código
- **JavaScript**: Camel case para variáveis/funções, Pascal case para objetos
- **CSS**: BEM methodology para classes
- **HTML**: Semântico e acessível
- **Comentários**: JSDoc para funções importantes

### Testes
- Testes manuais de funcionalidades
- Validação de cálculos com fontes externas
- Testes de responsividade

## 🤝 Como Contribuir

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas mudanças (`git commit -am 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

### Possíveis Melhorias
- [ ] Adicionar mais cidades e rotas
- [ ] Implementar API de mapas para distâncias reais
- [ ] Adicionar testes automatizados
- [ ] Suporte a múltiplos idiomas
- [ ] Integração com APIs de carbono
- [ ] PWA (Progressive Web App)

## 📊 Dados Técnicos

### Fatores de Emissão (kg CO₂/km)
- **Bicicleta**: 0 kg
- **Carro**: 0.12 kg
- **Ônibus**: 0.089 kg
- **Caminhão**: 0.96 kg

### Créditos de Carbono
- **Compensação**: 1 crédito = 1000 kg CO₂
- **Preço Estimado**: R$ 50 - R$ 150 por crédito

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 🙏 Agradecimentos

- Desenvolvido como projeto do curso da DIO (Digital Innovation One)
- Inspirado em iniciativas de sustentabilidade global
- Dados de emissões baseados em fontes científicas

---

**Desenvolvido com ❤️ para um planeta mais sustentável**