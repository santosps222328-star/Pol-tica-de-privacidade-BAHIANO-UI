# Política de Privacidade — BAHIANO UI >_♡

**Versão da extensão:** (Visível na Google Web Store)

> Esta política pode ser atualizada.

---

## Índice

1. [Resumo](#1-resumo)
2. [Dados usados pela extensão](#2-dados-usados-pela-extensão)
3. [Localização](#3-localização)
4. [Permissões da extensão](#4-permissões-da-extensão)
5. [Serviços externos](#5-serviços-externos)
6. [Onde seus dados ficam](#6-onde-seus-dados-ficam)
7. [O que nunca fazemos](#7-o-que-nunca-fazemos)
8. [Seus controles](#8-seus-controles)
9. [Segurança](#9-segurança)
10. [Crianças](#10-crianças)
11. [Alterações nesta política](#11-alterações-nesta-política)
12. [Contato](#12-contato)

---

## 1. Resumo

- A **BAHIANO UI >_♡** substitui a página de nova aba do Chrome por uma tela inicial com atalhos, pesquisa, relógio, clima, tradutor, gerador de QR Code, gerador de senhas, bloco de notas, tarefas e outras ferramentas.
- **Não vendemos** dados.
- **Não compartilhamos** dados com anunciantes, corretoras de dados ou terceiros para publicidade.
- O desenvolvedor **não possui servidor** que recebe dados da extensão. Não há conta, cadastro, login nem integração com contas Google.
- Suas configurações ficam salvas **no seu próprio navegador**.
- A extensão **não tem anúncios, rastreadores, cookies de publicidade nem ferramentas de análise** (como Google Analytics).
- Quando um recurso precisa de um serviço externo (por exemplo, o clima), **apenas o mínimo necessário** é enviado, e **somente quando você usa esse recurso**. Todos os casos estão na [seção 5](#5-serviços-externos).

---

## 2. Dados usados pela extensão

A extensão só trabalha com os dados abaixo, e apenas para o funcionamento dos recursos que você escolhe usar:

- **Localização** (aproximada ou GPS), somente se você permitir e clicar no botão de localização do widget de clima.
- **Texto digitado** nos campos de pesquisa, tradutor, QR Code e cidade do clima.
- **Preferências e configurações** (tema, atalhos, idioma, notas, tarefas, plano de fundo etc.).
- **Imagens de plano de fundo** que você escolher (ficam no seu navegador).

---

## 3. Localização

A localização é usada **somente** para mostrar o **clima** da sua região na tela inicial. Ela não é usada para publicidade, perfilamento, rastreamento, histórico de deslocamentos ou qualquer outra finalidade.

### 3.1 Como a localização é obtida

1. **GPS / localização do navegador (com sua permissão).** Ao clicar no botão de GPS do widget de clima, o Chrome pede sua autorização. Se você negar, nada é obtido, e você pode digitar o nome de uma cidade.
2. **Estimativa automática de cidade.** Se ainda não houver cidade salva, a extensão consulta o BigDataCloud, que estima sua cidade de forma aproximada a partir do **endereço IP** da sua conexão. Nesse caso, o GPS **não** é usado.
3. **Cidade digitada por você.** Nesse caso, a extensão não precisa da sua localização.

### 3.2 O que acontece com os dados de localização

| Etapa | O que acontece |
|---|---|
| Obtenção | Latitude e longitude são lidas pelo navegador, no seu dispositivo. |
| Nome da cidade | As coordenadas (ou o IP, na estimativa automática) são enviadas ao **BigDataCloud** (`api.bigdatacloud.net`), somente para converter em nome de cidade. |
| Clima | As coordenadas são enviadas ao **Open-Meteo** (`api.open-meteo.com`), somente para obter a previsão do tempo. |
| Armazenamento | Cidade e coordenadas escolhidas ficam **apenas no armazenamento local do seu navegador**, para não precisar buscar de novo a cada nova aba. |
| Servidores do desenvolvedor | **Nenhum.** O desenvolvedor não recebe e não tem acesso a esses dados. |

Esses serviços recebem apenas a requisição técnica necessária para responder (coordenadas e, se aplicável, o endereço IP) e têm políticas próprias:

- Open-Meteo: <https://open-meteo.com/en/terms>
- BigDataCloud: <https://www.bigdatacloud.com/privacy>

---

## 4. Permissões da extensão

| Permissão | Para que serve |
|---|---|
| `storage` e `unlimitedStorage` | Salvar suas configurações e dados dentro do próprio navegador, sem limite de espaço para imagens de fundo e backups locais. |
| `geolocation` | Obter sua localização para o clima. Só é usada se você permitir. |
| Acesso a 6 serviços (`host_permissions`) | Permite consultar apenas os serviços listados na [seção 5](#5-serviços-externos), e só quando o recurso correspondente é usado. |

---

## 5. Serviços externos

A extensão se comunica **somente** com os serviços abaixo. Cada um é acionado apenas quando o recurso correspondente é usado.

### 5.1 Clima e localização

| Serviço | Host | Quando | O que é enviado | Finalidade |
|---|---|---|---|---|
| Open-Meteo | `api.open-meteo.com` | Ao carregar o widget de clima. | Latitude e longitude da cidade escolhida ou da sua localização. | Temperatura, umidade, vento, máxima e mínima do dia. |
| Open-Meteo Geocoding | `geocoding-api.open-meteo.com` | Quando você digita o nome de uma cidade. | O nome da cidade digitada. | Encontrar as coordenadas da cidade. |
| BigDataCloud | `api.bigdatacloud.net` | Ao usar o botão de GPS (com sua permissão) e, na primeira abertura com o clima ativo e sem cidade salva, para estimar a cidade. | Coordenadas (botão de GPS) ou apenas o endereço IP (estimativa automática). | Transformar coordenadas em nome de cidade. |

### 5.2 Tradutor

| Serviço | Host | Quando | O que é enviado | Finalidade |
|---|---|---|---|---|
| MyMemory | `api.mymemory.translated.net` | Ao clicar em "Traduzir". | O texto digitado (até 480 caracteres) e os idiomas de origem e destino. | Devolver a tradução. |

> **Atenção:** o texto segue para esse serviço. Não digite dados sensíveis no tradutor.

### 5.3 Gerador de QR Code

| Serviço | Host | Quando | O que é enviado | Finalidade |
|---|---|---|---|---|
| QR Server | `api.qrserver.com` | Ao clicar em "Gerar QR Code". | O texto ou link que você digitou. | Gerar a imagem do QR Code. |

### 5.4 Sugestões de pesquisa

| Serviço | Host | Quando | O que é enviado | Finalidade |
|---|---|---|---|---|
| Google (sugestões) | `suggestqueries.google.com` | Enquanto você digita na barra de pesquisa da tela inicial. | O texto que você está digitando e o idioma da extensão. Não inclui cookies nem credenciais da sua conta Google. | Mostrar sugestões de pesquisa. |

- O histórico de pesquisas usado nas sugestões fica **somente no seu navegador**.
- Se não quiser sugestões, basta não digitar na barra de pesquisa.
- Política do Google: <https://policies.google.com/privacy>

### 5.5 Ícones dos atalhos

| Serviço | Quando | O que é enviado | Finalidade |
|---|---|---|---|
| Serviço de favicons do Google (`www.google.com/s2/favicons`) | Ao exibir os ícones dos seus atalhos. | O domínio do site do atalho (por exemplo, `youtube.com`). | Mostrar o ícone do site. |

### 5.6 Fontes

| Serviço | Quando | O que é enviado |
|---|---|---|
| Google Fonts (`fonts.googleapis.com`, `fonts.gstatic.com`) | Ao abrir a tela inicial. | Requisição padrão para baixar as fontes Inter e Orbitron. Nenhum dado pessoal. |

### 5.7 Imagem de plano de fundo por link

- Se você colar o endereço de uma imagem como plano de fundo, o navegador baixa a imagem diretamente desse endereço. Esse site pode registrar a sua conexão, como qualquer acesso a um site comum.

---

## 6. Onde seus dados ficam

- Configurações, atalhos, notas, tarefas, idioma, cidade do clima e plano de fundo ficam no **armazenamento local do navegador** (`localStorage` e `IndexedDB`).
- Esses dados **não são enviados ao desenvolvedor**.
- Backups são arquivos `.json` que **você** exporta e guarda onde quiser. A extensão não envia esses arquivos a lugar nenhum.
- Ao remover a extensão do Chrome, os dados locais são apagados.

---

## 7. O que nunca fazemos

- Não vendemos dados pessoais.
- Não alugamos, não trocamos e não publicamos dados de usuários.
- Não usamos dados para publicidade, perfil de consumo, crédito ou empréstimos.
- Não coletamos histórico de navegação do Chrome nem histórico da sua conta Google.
- Não acessamos suas abas, senhas, cookies ou arquivos.
- Não temos acesso remoto ao seu computador ou ao seu navegador, e a extensão não recebe comandos remotos.
- Não guardamos seus dados em servidores do desenvolvedor.

---

## 8. Seus controles

- **Localização:** negue ou revogue a permissão em *Configurações do Chrome → Privacidade e segurança → Configurações de sites → Localização*, ou pelo ícone de cadeado/permissões na nova aba. Sem a permissão, basta digitar a cidade.
- **Clima:** pode ser desativado nas configurações da extensão.
- **Sugestões de pesquisa:** não digite na barra de pesquisa se não quiser usá-las.
- **Apagar tudo:** remova a extensão em `chrome://extensions`.

---

## 9. Segurança

- As comunicações com os serviços externos usam **HTTPS**.
- A extensão **não pede senhas, dados bancários nem documentos**.
- A extensão **não tem área de login** e não integra contas Google.

---

## 10. Crianças

A extensão não é direcionada a crianças e não coleta intencionalmente dados pessoais de menores de idade.

---

## 11. Alterações nesta política

Se a extensão passar a usar novos serviços ou novos tipos de dados, esta política será atualizada e a nova data aparecerá no topo do documento. Recomendamos a leitura periódica.

---

## 12. Contato

Dúvidas sobre privacidade: **[SEU E-MAIL DE CONTATO]**

Repositório desta política: <https://github.com/santosps222328-star/Pol-tica-de-privacidade-BAHIANO-UI>

---

## Resumo final

A BAHIANO UI não vende dados, não tem servidor que recebe seus dados, não tem acesso remoto ao seu navegador e não usa rastreadores nem anúncios. Cada serviço externo listado acima recebe apenas o mínimo necessário para o recurso que você usou, e você decide quando usar cada um.
