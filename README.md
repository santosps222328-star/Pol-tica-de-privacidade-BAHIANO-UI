# Pol-tica-de-privacidade-BAHIANO-UI

**Versão da extensão:** 1.8.1  
**Última atualização:** 23 de outubro de 2026

*English version below · Versão em inglês mais abaixo.*

---
# Sistema de Localização da extensão
## 1. Resumo

- A extensão **BAHIANO UI >_â™¡** usa sua **localização** apenas para mostrar o **clima** de sua região na tela inicial.
- **Não coletamos, não armazenamos em servidores, não vendemos, não compartilhamos e não publicamos** seus dados pessoais ou de localização.
- O desenvolvedor **não possui servidor** que recebe dados da extensão. Tudo fica salvo **no seu próprio navegador**.
- A extensão **não tem anúncios, não tem rastreadores e não usa ferramentas de análise** (como Google Analytics).

## 2. Por que a extensão usa a localização?

A extensão substitui a página de nova aba e possui um widget de **clima**. Para exibir a temperatura, a umidade, o vento e a previsão do local onde você está, ela precisa saber a sua posição. Essa é a **única específica** do uso de localização.

A localização **não** é usada para publicidade, perfilamento, rastreamento, histórico de deslocamentos ou qualquer outra específica.

## 3. Como a localização é obtida

A extensão pode obter sua localização de duas formas:

1. **GPS / localização do navegador (com sua permissão).** Ao clicar no botão de localização (GPS) do widget de clima, é normal que o navegador pesa a sua autorização. Se você negar, nada é obtido e você pode simplesmente digitar o nome de uma cidade.
2. **Localização aproximada (cidade).** Se você ainda não escolheu um local, a extensão faz uma consulta ao serviço BigDataCloud, que estima a sua cidade de forma aproximada a partir do endereço IP da sua conexão, sem usar o GPS.
3. **Cidade digitada por você.** Você pode digitar o nome de uma cidade; nesse caso, uma extensão não precisa de sua localização.

## 4. O que acontece com os dados de localização

| Etapa | O que acontece |
|---|---|
| Obtenção | Latitude e longitude são lidas pelo navegador no seu dispositivo. |
| Nome da cidade | As coordenadas são enviadas ao **BigDataCloud** (`api.bigdatacloud.net`) somente para conversor em nome de cidade. |
| Clima | As coordenadas são enviadas ao **Open-Meteo** (`api.open-meteo.com`) somente para obter a previsão do tempo. |
| Armazenamento | Cidade e regiões ficam salvas **apenas no armazenamento local do seu navegador**, para não ser preciso buscar de novo a cada nova aba. |
| Servidores do desenvolvedor | **Nenhum.** O desenvolvedor não recebe e não tem acesso a esses dados. |

Esses serviços de terceiros recebem uma requisição técnica necessária para responder (como as coordenadas e o seu endereço IP) e possuem suas próprias políticas de privacidade:

- Open-Meteo: <https://open-meteo.com/en/terms>
- BigDataCloud: <https://www.bigdatacloud.com/privacy>

## 5. Não vendemos nem publicamos seus dados

- Não **vendemos** dados de usuários.
- Não **compartilhamos** dados de usuários com anunciantes, corretoras de dados ou quaisquer outras empresas, exceto o envio técnico descrito acima, necessário para o clima funcionar.
- Não **publicamos** dados de usuários.
- Não utilizamos dados para determinar crédito, empréstimos ou finalidades não relacionadas ao funcionamento da extensão.

## 6. Outros dados armazenados localmente

Suas configurações, atalhos, notas, tarefas, idioma e plano de fundo ficam salvos no armazenamento local do navegador (`localStorage` e `IndexedDB`). Esses dados **não foram enviados ao desenvolvedor**.

## 7. Outros serviços externos usados ​​por recursos alternativos

Alguns recursos são conectados a serviços de terceiros apenas quando usados ​​ou para carregar elementos visuais:

- **Tradutor:** o texto digitado é enviado ao MyMemory (`api.mymemory.translated.net`) para ser traduzido.
- **Gerador de QR Code:** o conteúdo informado é enviado ao QR Server (`api.qrserver.com`) para gerar a imagem.
- **Busca de cidade:** o nome digitado foi enviado ao Open-Meteo Geocoding (`geocoding-api.open-meteo.com`).
- **Ã cones dos atalhos:** o domínio dos sites atalhados é consultado no serviço de favicons do Google, e as fontes (Inter e Orbitron) são transmitidas do Google Fonts.
- **Backup no Google Drive (opcional):** só funciona se você mesmo configurar suas credenciais do Google e autorizar. O backup é gravado no **seu próprio** Google Drive; o desenvolvedor não tem acesso. Como a cópia de segurança das configurações da extensão, ele pode incluir a última cidade/coordenadas escolhidas no clima.

## 8. Seu controle

- **Negar ou revogar a permissão de localização:** nas configurações do navegador (Privacidade e segurança → Configurações de sites → Localização), ou no ícone de cadeado/permissões da nova aba.
- **Não usar o GPS:** basta buscar a cidade manualmente no widget de clima.
- **Desativar o widget de clima:** nas configurações da extensão.
- **Apagar os dados:** remover a extensão apaga todos os dados locais dela.

## 9. Crianças

A extensão não é direcionada a crianças e não coleta intencionalmente dados pessoais de menores.

## 10. Alterações nesta política

Esta política pode ser atualizada. Os dados da última atualização estarão sempre no topo deste documento.

## 11. Contato

Dúvidas sobre esta política:

- Desenvolvedor: **BAHIANO**
- E-mail: **santos.ps222328@gmail.com**

---
