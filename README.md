# ABC Parts — Expedição e Separação

App de celular (PWA) para a separação de material no estoque da ABC Parts.
O operador lê o QR do **PV**, o cronômetro inicia, ele lê o QR da etiqueta de
cada item — registrando o **número de rastreabilidade** (pedido de compra) —
e ao finalizar o app grava a **duração da separação** e a **data/hora em que o
PV ficou liberado para produção**.

| Arquivo | O que é |
|---|---|
| [`expedicao.html`](expedicao.html) | O app. Página única, sem build. |
| [`index.html`](index.html) | Entrada do site: redireciona para o app. |
| [`sw-expedicao.js`](sw-expedicao.js) | Service worker — o app funciona sem conexão. |
| [`vendor/jsQR.min.js`](vendor/jsQR.min.js) | Leitor de QR usado no iPhone e onde não há `BarcodeDetector`. Cópia local, sem CDN. |
| [`apps-script/expedicao.gs`](apps-script/expedicao.gs) | Endpoint do Google Sheets que recebe as separações. |
| [`docs/expedicao.md`](docs/expedicao.md) | Instalação, configuração e layout das colunas. |

## Como abrir

Publicado por GitHub Pages em **https://denismazzoni.github.io/abc-parts/**

No iPhone, abra no **Safari** e use *Compartilhar › Adicionar à Tela de Início*
para instalar. No Android, é *Instalar aplicativo* no menu do Chrome.

Detalhes de uso e configuração: [`docs/expedicao.md`](docs/expedicao.md).
