# Babá Inteligente com BitDogLab (Raspberry Pi Pico W) – Monitoramento de Som em Tempo Real👨🏻‍💻🤱🏻

Este projeto implementa uma **Babá Eletrônica** utilizando a placa **BitDogLab**. Ele monitora sons no ambiente e executa ações específicas, como exibir informações no display OLED e alertar por meio de LEDs RGB e um buzzer, permitindo a identificação do ambiente.

🎥 **Vídeo Demonstrativo:**  
[Assista ao vídeo aqui](https://drive.google.com/file/d/1dHTUrqbrFajbe9q0Wo3BTwAEuXMR_DhR/view?usp=sharing)

## 📌 Descrição do Projeto

A Babá Eletrônica detecta sons e fornece feedback visual e auditivo sobre o estado do ambiente. O sistema é controlado por botões físicos que permitem ativar e desativar a detecção de som.

### Funcionalidades

- **Detecção de Som:** Identifica ruídos no ambiente com um microfone analógico.
- **Reprodução de Melodia:** Toca "Brilha, Brilha Estrelinha" no buzzer ao detectar som.
- **Indicadores Visuais:**
  - 🔵 **Azul:** Sistema aguardando ativação.
  - 🟢 **Verde:** Sistema ativo.
  - 🔴 **Vermelho:** Sistema Desativado.
 
- **Controle por Botões:**
  - **Botão A:** Ativa o sistema.
  - **Botão B:** Desativa o sistema.
- **Display OLED:** Exibe mensagens sobre o status do sistema.

## 🛠 Requisitos

### 📌 Hardware Necessário

- Raspberry Pi Pico W
- Display OLED SSD1306
- Buzzer Passivo
- Microfone Analógico
- Botões (2 unidades)
- LED RGB
- Protoboard e Jumpers

### 💾 Software Necessário

- Raspberry Pi Pico SDK
- Biblioteca SSD1306
- **Ferramentas de Desenvolvimento:**
  - Visual Studio Code com extensões para C/C++ e Pico SDK
  - CMake para geração de builds

## 📂 Estrutura do Projeto

```
CEPEDI_PROJETO_FINAL/
├── CMakeLists.txt        # Configuração do CMake
├── display_oled.c        # Código principal
├── inc/
│   ├── ssd1306.h        # Header do display OLED
│   ├── ssd1306.c        # Driver do display OLED
└── README.md            # Documentação do projeto
```

## 🚀 Como Usar

### 1️⃣ Configuração de Hardware

Conecte os componentes conforme descrito na seção de hardware.

### 2️⃣ Configuração de Software

Compile o código utilizando o CMake:
```sh
mkdir build && cd build
cmake ..
make
```

### 3️⃣ Upload para a Raspberry Pi Pico

- Conecte sua Pico W via USB enquanto pressiona o botão **BOOTSEL**.
- Solte o botão e uma unidade USB aparecerá no seu computador.
- Arraste e solte o arquivo `.uf2` gerado para a unidade.

####  - 💡 Criado e Desenvolvido por : [Everton Espedito Silva Santos](https://www.linkedin.com/in/everton-espedito-3062071a3/)
