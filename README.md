Bitcoin Testnet Wallet Generator
Este projeto é um gerador de carteiras Bitcoin na rede Testnet. Ele cria pares de chave pública e privada, além de gerar um endereço Bitcoin que pode ser usado para enviar e receber transações na Testnet.

Funcionalidades
Gera um endereço Bitcoin na Testnet.
Suporta diferentes formatos de endereços (P2PKH, P2SH-P2WPKH, e P2WPKH).
Exporta a chave privada (WIF) e o seed (mnemônico) para importação em outras carteiras.
Tecnologias Utilizadas
Node.js
bitcoinjs-lib
bip32
bip39
Como Usar
Clone o repositório:

bash
Copiar código
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
Instale as dependências:

bash
Copiar código
npm install
Execute o script:

bash
Copiar código
node walletGenerator.js
Verifique a saída:

O script exibirá o endereço Bitcoin gerado, a chave privada (WIF) e o seed (mnemônico) no console.

Endereço: Pode ser usado na Testnet para enviar e receber bitcoins de teste.
Chave Privada: Use para importar a carteira em aplicativos como Electrum.
Seed: Pode ser usado para restaurar a carteira em diferentes dispositivos.
Tipos de Endereços Suportados
P2PKH (Legacy): Caminho de derivação m/44'/1'/0'/0/0. Endereços que começam com m ou n.
P2SH-P2WPKH (SegWit compatível): Caminho de derivação m/49'/1'/0'/0/0. Endereços que começam com 2.
P2WPKH (SegWit nativo): Caminho de derivação m/84'/1'/0'/0/0. Endereços que começam com tb1.
Importação no Electrum
Abra o Electrum e selecione "Create new wallet".
Escolha "Import Bitcoin addresses or private keys".
Cole a chave privada (WIF) gerada pelo script.
Finalize e comece a usar sua carteira.
Obtendo Bitcoins de Teste
Para enviar bitcoins de teste para o seu endereço, use um faucet Testnet.

Licença
Este projeto é licenciado sob os termos da MIT License.
