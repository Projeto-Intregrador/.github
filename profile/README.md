# InfasCare IoT

Bem-vindo ao InfasCare IoT!

O InfasCare IoT é um sistema inteligente de monitoramento e prevenção ao abandono infantil em veículos, desenvolvido por meio da integração entre Internet das Coisas (IoT), geolocalização, computação em nuvem e inteligência artificial.

A solução tem como objetivo aumentar a segurança infantil em automóveis através de uma arquitetura inteligente capaz de detectar a presença da criança na cadeirinha, identificar o afastamento do responsável e gerar alertas preventivos em tempo real.

O sistema foi projetado para atuar de forma preventiva, reduzindo riscos relacionados ao esquecimento infantil em veículos fechados.

---

# Objetivo

O projeto tem como objetivo desenvolver uma solução IoT aplicada à segurança infantil automotiva, utilizando sensores inteligentes, análise de comportamento e monitoramento remoto para prevenir situações de risco envolvendo crianças esquecidas em veículos.

---

# Contexto

Casos de abandono infantil em veículos representam um problema grave de segurança pública em diversos países. Em muitos cenários, alterações de rotina, distrações e falhas humanas contribuem para que responsáveis esqueçam crianças dentro do automóvel.

Soluções existentes normalmente dependem apenas de sensores simples ou conexões Bluetooth de curto alcance, limitando a capacidade preventiva do sistema.

O InfasCare IoT propõe uma abordagem híbrida baseada em:

* monitoramento inteligente;
* análise de rotina;
* localização do responsável;
* processamento em nuvem;
* alertas progressivos em tempo real.

---

# Modelo da Solução

O sistema é composto por uma arquitetura distribuída dividida em:

## Módulo IoT da Cadeirinha

Responsável pela coleta de informações físicas.

Funções:

* detectar presença da criança;
* monitorar temperatura interna;
* enviar dados para a nuvem;
* acionar alertas locais.

## Aplicativo Mobile

Responsável pela interação com os responsáveis.

Funções:

* receber notificações;
* exibir status da cadeirinha;
* compartilhar localização;
* registrar histórico de eventos;
* confirmar retirada da criança.

## Plataforma em Nuvem

Responsável pelo armazenamento e processamento dos dados.

Funções:

* autenticação de usuários;
* armazenamento de dados;
* processamento das regras de risco;
* envio de notificações.

## Módulo de Inteligência Artificial

Responsável pela análise de comportamento.

Funções:

* identificar horários incomuns;
* analisar padrões de rotina;
* detectar possíveis situações de risco;
* gerar alertas preventivos.

---

# Funcionalidades

## Monitoramento da Cadeirinha

* detecção de presença infantil;
* monitoramento contínuo;
* verificação do status da cadeirinha.

## Controle de Temperatura

* leitura da temperatura interna do veículo;
* alertas preventivos;
* classificação de risco térmico.

## Sistema de Localização

* monitoramento da distância do responsável;
* integração com GPS do smartphone;
* verificação de proximidade em tempo real.

## Inteligência Artificial

* análise de padrões de uso;
* identificação de horários incomuns;
* geração de alertas preventivos;
* classificação automática de risco.

## Sistema de Alertas

* notificações push;
* alerta sonoro local;
* alertas progressivos;
* contato secundário em situações críticas.

---

# Arquitetura do Sistema

```text
[Cadeirinha Inteligente]
        |
        | Sensores
        v
[ESP32]
        |
        | Wi-Fi / Bluetooth
        v
[Firebase / Nuvem]
        |
        | Processamento IA
        v
[Aplicativo Mobile]
        |
        v
[Responsável]
```

---

# Estrutura Física

O protótipo físico será composto pelos seguintes módulos:

## Módulo Inteligente da Cadeirinha

Composto por:

* ESP32;
* sensor de presença/peso;
* sensor de temperatura;
* módulo de comunicação Wi-Fi/Bluetooth.

## Aplicativo Mobile

Desenvolvido em React Native para:

* monitoramento em tempo real;
* recebimento de alertas;
* compartilhamento de localização;
* gerenciamento de notificações.

---

# Tecnologias Utilizadas

## Hardware

* ESP32
* Sensor de presença
* Sensor de temperatura
* Bluetooth Low Energy (BLE)

## Software

* React Native
* Firebase
* Firebase Authentication
* Firestore Database
* Firebase Cloud Messaging

## Inteligência Artificial

* análise comportamental;
* processamento de padrões de rotina;
* classificação de risco.

---

# Regras de Funcionamento

## Situação Normal

```text
Criança presente + responsável próximo
```

## Situação de Atenção

```text
Criança presente + horário fora da rotina
```

## Situação de Risco

```text
Criança presente + responsável distante
```

## Situação Crítica

```text
Criança presente + responsável distante + temperatura elevada
```

---

# Fluxo Operacional

```text
1. Sensor detecta presença da criança
2. ESP32 envia dados para a nuvem
3. Aplicativo compartilha localização do responsável
4. IA analisa padrões de rotina
5. Sistema identifica possíveis riscos
6. Firebase envia alertas em tempo real
7. Alerta sonoro local é acionado
```

---

# Diferenciais do Projeto

O InfasCare IoT diferencia-se por integrar:

* IoT;
* geolocalização;
* computação em nuvem;
* análise inteligente de rotina;
* monitoramento preventivo.

A proposta não depende apenas de sensores simples, mas utiliza análise contextual para identificar situações de risco antes que elas se tornem críticas.

---

# Estrutura do Projeto

```text
InfasCare-IoT/
│
├── mobile-app/
├── firmware-esp32/
├── backend-firebase/
├── docs/
├── diagrams/
├── prototypes/
└── README.md
```

---

# Futuras Implementações

* integração com smartwatch;
* dashboard analítico;
* integração com veículos conectados;
* machine learning avançado;
* sistema automatizado de emergência.

---

# Segurança

O sistema utiliza:

* autenticação segura;
* comunicação HTTPS;
* controle de acesso aos dados;
* criptografia de informações sensíveis.

---

# Protótipo

O protótipo será desenvolvido utilizando modelagem 3D e impressão de componentes físicos para integração à cadeirinha infantil.

O dispositivo será projetado de forma não invasiva, garantindo segurança, conforto e facilidade de instalação.

---

# Governança do Projeto

O projeto é desenvolvido para fins acadêmicos e de pesquisa tecnológica, com foco em inovação aplicada à segurança infantil automotiva.

---

# Versionamento

O projeto seguirá versionamento semântico para organização e controle das evoluções do sistema.

---

# Contato

Em caso de dúvidas ou sugestões:

* Yasmin Oliveira
* Letícia Borges
* João Machado

---

# Referências

Referência consultada para estruturação documental e arquitetura de apresentação institucional: 

---

# Licença

Projeto acadêmico desenvolvido para fins educacionais, científicos e de pesquisa tecnológica.
