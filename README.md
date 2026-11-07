# Diagnóstico de Transformação Digital

> **Aplicativo Web Interativo para Avaliação de Maturidade Tecnológica, Análise de Riscos e Emissão de Laudo Estratégico com Gráfico Radar.**

---

## 📌 Visão Geral

O **Diagnóstico de Transformação Digital** é uma ferramenta interativa desenvolvida para consultores de TI, diretores de tecnologia (CTOs), gerentes de inovação e gestores de pequenas, médias e grandes empresas (PMEs). 

O sistema avalia a maturidade digital em **4 pilares fundamentais**, calcula instantaneamente a pontuação global e setorial em tempo real, projeta um **Gráfico Radar multidimensional** e gera um **Laudo Técnico Executivo** com matriz de severidade e um **Roadmap de Ação para 30, 60 e 90 dias**.

---

## 🌟 Principais Funcionalidades

- **Diagnóstico em Tempo Real (Sem Recarregar):** Cálculo instantâneo do score geral (0% a 100%) e das dimensões à medida que as opções são selecionadas.
- **Gráfico Radar Interativo (Chart.js):** Projeção visual dos 4 eixos estratégicos para identificar desequilíbrios na operação.
- **12 Perguntas Didáticas:** 3 questões por pilar com explicações para leigos em itálico (*o que significa e por que importa*).
- **Botão Demo ("Carregar Caso Exemplo"):** Preenche automaticamente o cenário clássico de dependência de servidor físico local, planilhas Excel desconectadas e ausência de CRM/LGPD.
- **Laudo Técnico com Alertas de Cores Vibrantes:**
  - 🚨 **Riscos Graves (`bg-rose-500`):** Vulnerabilidades críticas com risco iminente de prejuízo, sequestro de dados ou paralisia da empresa.
  - ⚠️ **Pontos de Atenção (`bg-amber-400`):** Processos manuais, ferramentas isoladas e gargalos de produtividade.
  - ✅ **Boas Práticas (`bg-emerald-500`):** Reconhecimento das fortalezas e tecnologias maduras já adotadas.
- **Roadmap Tático (30, 60 e 90 Dias):** Plano de ação cronológico sugerido para guiar a tomada de decisão da diretoria.
- **Modo de Impressão / Exportação em PDF:** Estilos CSS `@media print` otimizados para gerar um relatório executivo formal em papel/PDF, ocultando botões e navegação.
- **Privacy by Design:** Todo o processamento ocorre 100% no navegador do usuário (*client-side*). Nenhum dado corporativo ou resposta é transmitido para servidores externos.

---

## 🧱 Os 4 Pilares da Avaliação

O diagnóstico está estruturado nos quatro alicerces da empresa digital moderna:

| Pilar | Imagem Representativa | Ícone FontAwesome | Foco Estratégico |
| :--- | :--- | :---: | :--- |
| **1. Nuvem & Infraestrutura** | `seed/cloud/400/200` | `<i class="fa-solid fa-cloud"></i>` | Hospedagem elástica, rotina de backups/DRP e trabalho remoto seguro. |
| **2. ERP, CRM & Dados** | `seed/data/400/200` | `<i class="fa-solid fa-database"></i>` | Unificação financeira/estoque, pipeline de vendas e Business Intelligence (BI). |
| **3. IA & Automação** | `seed/robot/400/200` | `<i class="fa-solid fa-robot"></i>` | Workflows/RPA, atendimento inteligente e governança de IA generativa. |
| **4. Segurança & LGPD** | `seed/lock/400/200` | `<i class="fa-solid fa-shield-halved"></i>` | MFA/2FA, conformidade com a Lei 13.709/2018, antivírus corporativo (EDR) e treinamento humano. |

---

## 📊 Matriz de Maturidade Digital

A pontuação total é calculada com base em 12 perguntas (0 a 3 pontos cada, totalizando 36 pontos possíveis):

| Faixa (%) | Nível | Descrição Executiva |
| :---: | :--- | :--- |
| **0% – 30%** | **Nível 1: Inicial / Crítico** | Alta vulnerabilidade operacional. Dependência de servidores físicos obsoletos, planilhas soltas e ausência de segurança básica. |
| **31% – 60%** | **Nível 2: Operacional / Parcial** | Ferramentas pontuais em uso, mas com ilhas isoladas de informação e retrabalho manual frequente. |
| **61% – 85%** | **Nível 3: Estruturado / Integrado** | Infraestrutura em nuvem e sistemas de gestão consolidados. Foco na expansão de automação e dados analíticos. |
| **86% – 100%** | **Nível 4: Inovador / Data-Driven** | Excelência tecnológica, governança contínua, processos autônomos e IA integrada ao core business. |

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído para ser **autossuficiente, leve e portável**, podendo ser executado em qualquer ambiente sem necessidade de banco de dados externo ou backend complexo:

- **HTML5 Semântico:** Estruturação acessível com componentes modulares.
- **TailwindCSS (via CDN):** Estilização visual contemporânea, tipografia com alto contraste suave e paleta de alertas vibrantes.
- **Chart.js (via CDN):** Renderização vetorial responsiva do Gráfico Radar com atualização dinâmica via JavaScript.
- **FontAwesome 6 (via CDN):** Ícones vetoriais representativos de cada conceito tecnológico.
- **JavaScript Vanilla (ES6+):** Lógica reativa pura para cálculo de pontuações, listeners de eventos e geração dinâmica do laudo.

---

## 🚀 Como Executar o Projeto

### Opção 1: Execução Direta (Sem Instalação)
Por se tratar de uma aplicação autossuficiente em arquivo único (`index.html`), basta:
1. Clonar ou baixar o repositório.
2. Clicar duas vezes no arquivo `index.html` ou abri-lo diretamente em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).

### Opção 2: Execução com Servidor de Desenvolvimento (Vite / Node.js)
Caso deseje rodar através do ecossistema Node já presente no projeto:

```bash
# 1. Instalar dependências (se necessário)
npm install

# 2. Iniciar o servidor local de desenvolvimento
npm run dev

# 3. Acesse a URL exibida no terminal (geralmente http://localhost:3000)
```

---

## 🖨️ Exportação em PDF e Impressão

Para gerar o relatório executivo para apresentação a sócios ou diretoria:
1. Preencha o perfil da empresa e as 12 questões (ou clique em **"Carregar Caso Exemplo (Demo)"**).
2. Clique no botão **"Imprimir / Salvar PDF"** no topo da tela.
3. No diálogo de impressão do navegador, selecione **"Salvar como PDF"** ou a impressora desejada.
4. O CSS `@media print` automaticamente:
   - Remove botões de ação e banners promocionais.
   - Aplica cabeçalho executivo formal com data e hora da emissão.
   - Ajusta o tamanho do gráfico radar e impede quebras de página inadequadas no laudo técnico.

---

## 🔒 Soberania dos Dados & LGPD (Privacy by Design)

- **Processamento 100% Client-Side:** Todas as operações matemáticas, diagnósticos e relatórios são executados localmente na memória RAM do navegador.
- **Sem Rastreamento:** Nenhuma informação preenchida (nome da empresa, faturamento, respostas operacionais) é gravada em bancos de dados em nuvem ou enviada para serviços de terceiros.
- **Segurança da Informação:** A conformidade com a LGPD e o sigilo de segredos industriais da empresa estão garantidos por arquitetura de software.

---

## 📄 Licença

Distribuído sob a licença **Apache 2.0**. Consulte o arquivo de licença correspondente para mais informações.

## Link da página: https://darthruver007.github.io/diagnostico_transformacao_digital/
