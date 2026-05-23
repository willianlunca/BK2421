# BK2421 KiCad Library

<div align="center">

![KiCad](https://img.shields.io/badge/KiCad-6%2F7%2F8-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![RF](https://img.shields.io/badge/RF-2.4GHz-orange)
![Status](https://img.shields.io/badge/Status-Active-success)

Biblioteca completa para o transceptor RF BK2421 contendo símbolo esquemático, footprint PCB e modelo 3D `.STEP` para utilização no KiCad.

</div>

---

# 📖 Sobre o Projeto

Este repositório foi criado com o objetivo de facilitar o desenvolvimento de hardware utilizando o chip **BK2421**, um transceptor RF 2.4GHz extremamente popular e compatível com diversos projetos baseados no protocolo do **nRF24L01**.

A biblioteca contém:

- ✅ Símbolo esquemático
- ✅ Footprint PCB
- ✅ Modelo 3D `.STEP`
- ✅ Compatibilidade com KiCad 6, 7 e 8
- ✅ Estrutura pronta para integração em projetos profissionais

---

# 📦 Estrutura do Repositório

```text
BK2421-KiCad-Library/
│
├── symbols/
│   └── BK2421.kicad_sym
│
├── footprints/
│   └── BK2421.pretty/
│       └── BK2421_QFN20.kicad_mod
│
├── 3dmodels/
│   └── BK2421.step
│
├── images/
│   ├── symbol.png
│   ├── footprint.png
│   ├── pcb_render.png
│   └── assembled.png
│
├── datasheet/
│   └── BK2421.pdf
│
└── README.md
```

---

# ✨ Recursos

## 🔷 Símbolo Esquemático

O símbolo foi desenvolvido seguindo a organização lógica do datasheet oficial:

- Alimentação separada
- GPIOs organizados
- SPI destacado
- Pinos RF identificados
- Compatível com ERC do KiCad

### Recursos:

- Compatível com KiCad moderno
- Nomeação padronizada
- Fácil leitura no esquemático
- Pino 1 identificado

---

## 🔶 Footprint PCB

Footprint desenvolvido para montagem SMD profissional.

### Características:

- Encapsulamento QFN
- Pad central exposto
- Compatível com fabricação industrial
- Silkscreen otimizado
- Marca de orientação do pino 1
- Compatível com montagem automatizada

### Baseado em:

- Datasheet oficial do BK2421
- Recomendações IPC
- Dimensões reais do encapsulamento

---

## 🟢 Modelo 3D `.STEP`

Modelo 3D criado para:

- Renderização no KiCad
- Verificação mecânica
- Compatibilidade com CAD 3D
- Integração MCAD/ECAD

Compatível com:

- KiCad
- Fusion 360
- SolidWorks
- FreeCAD
- Altium

---

# 📡 Sobre o BK2421

O **BK2421** é um transceptor RF de 2.4GHz utilizado em aplicações wireless de baixo custo e baixo consumo.

## Principais Características

| Característica | Valor |
|---|---|
| Frequência | 2.4GHz |
| Interface | SPI |
| Modulação | GFSK |
| Alimentação | 1.9V ~ 3.6V |
| Consumo reduzido | Sim |
| Comunicação bidirecional | Sim |
| Compatível com nRF24L01 | Sim |

---

# 🔄 Compatibilidade com nRF24L01

O BK2421 possui compatibilidade com diversos projetos originalmente desenvolvidos para o:

- nRF24L01
- nRF24L01+
- Módulos RF 2.4GHz populares

Isso facilita:

- Migração de projetos
- Reutilização de firmware
- Integração com bibliotecas existentes

---

# 🛠️ Como Instalar

# 1️⃣ Clonar o Repositório

```bash
git clone https://github.com/SEU_USUARIO/BK2421-KiCad-Library.git
```

---

# 2️⃣ Adicionar Biblioteca de Símbolos

No KiCad:

```text
Preferences → Manage Symbol Libraries
```

Clique em:

```text
Add Existing Library
```

Selecione:

```text
symbols/BK2421.kicad_sym
```

---

# 3️⃣ Adicionar Biblioteca de Footprints

No KiCad:

```text
Preferences → Manage Footprint Libraries
```

Selecione:

```text
footprints/BK2421.pretty
```

---

# 4️⃣ Associar Modelo 3D

Abra o footprint:

```text
Footprint Properties → 3D Models
```

Selecione:

```text
3dmodels/BK2421.step
```

---

# 🖼️ Imagens

## Símbolo

![Símbolo](images/symbol.png)

---

## Footprint

![Footprint](images/footprint.png)

---

## Renderização PCB

![PCB](images/pcb_render.png)

---

## Montagem 3D

![3D](images/assembled.png)

---

# 📐 Recomendações de Layout RF

Projetos RF exigem cuidados especiais no PCB.

## Recomendações

### ✅ Utilize plano de GND sólido

Preferencialmente:

- Camada inferior inteira GND
- Via stitching próximo ao chip

---

### ✅ Mantenha trilhas RF curtas

Evite:

- Trilhas longas
- Curvas agressivas
- Descontinuidades

---

### ✅ Matching RF

O circuito de matching deve ficar extremamente próximo ao chip.

Exemplo:

```text
BK2421 → Matching Network → Antena
```

---

### ✅ Capacitores de desacoplamento

Posicione:

- 100nF
- 1uF

O mais próximo possível dos pinos de alimentação.

---

# 📚 Aplicações

Esta biblioteca pode ser utilizada em:

- Sensores sem fio
- Automação industrial
- Telemetria
- IoT
- Comunicação MCU ↔ MCU
- Redes mesh
- Equipamentos embarcados
- Dispositivos alimentados por bateria

---

# 🔧 Compatibilidade

| Software | Compatível |
|---|---|
| KiCad 6 | ✅ |
| KiCad 7 | ✅ |
| KiCad 8 | ✅ |
| Fusion 360 | ✅ |
| FreeCAD | ✅ |
| SolidWorks | ✅ |

---

# 📁 Arquivos Inclusos

| Arquivo | Descrição |
|---|---|
| `.kicad_sym` | Símbolo esquemático |
| `.kicad_mod` | Footprint |
| `.step` | Modelo 3D |
| `.png` | Imagens |
| `.pdf` | Datasheet |

---

# 🤝 Contribuições

Contribuições são bem-vindas.

Você pode contribuir com:

- Correções
- Melhorias no footprint
- Modelos 3D
- Testes
- Exemplos de uso

---

# 📝 Licença

Este projeto é distribuído sob licença MIT.

Você pode utilizar:

- Projetos pessoais
- Projetos comerciais
- Desenvolvimento profissional

---

# ⭐ Apoie o Projeto

Se este projeto foi útil para você:

- ⭐ Dê uma estrela no GitHub
- 🍴 Faça um fork
- 📢 Compartilhe

---

# 🔗 Referências

## KiCad

- https://www.kicad.org/

## Repositórios de Referência

- https://github.com/KiCad
- https://github.com/sparkfun
- https://github.com/adafruit

---

# ⚠️ Aviso

Este projeto não possui vínculo oficial com o fabricante do BK2421.

As informações foram baseadas em:

- Datasheets públicos
- Medições reais
- Compatibilidade prática com nRF24L01

---

<div align="center">

Desenvolvido para a comunidade open-source ❤️

</div>
