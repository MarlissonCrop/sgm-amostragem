# 🌱 SGM Seeds — Controle de Amostragem

Sistema de controle de amostragem de sementes desenvolvido para o laboratório da **SGM Seeds**. Roda diretamente no navegador do celular ou tablet, sem necessidade de instalação.

---

## 🔗 Acesso

**[https://marlissoncrop.github.io/sgm-amostragem/sgm-amostragem.html](https://marlissoncrop.github.io/sgm-amostragem/sgm-amostragem.html)**

> Adicione à tela inicial do celular para acesso rápido como um app.

---

## 📋 Funcionalidades

### Cadastro de Lotes
- **Fotografia da etiqueta** com leitura automática via OCR (Google Vision API)
- Extração automática de: ID do lote, espécie, cultivar, cliente e RENASEM
- Correção manual dos campos quando necessário

### Gerenciamento de Bags
- Adição rápida de bag individual com um toque no botão `+`
- Adição em lote por intervalo (ex: bag 1 → 40) ou sequência (ex: bag 15 → 54)
- Edição e exclusão de bags com confirmação
- Registro do **responsável pela amostragem** por seleção rápida

### Controle de Etapas
Cada bag passa pelo seguinte fluxo:
```
Amostragem → Homo/Redução → Amostras de Trabalho
```
- Etapas marcadas com um toque
- Progresso visual por bag

### Amostras de Trabalho
Registro de quantidade por tipo de análise:
| Análise | Descrição |
|---------|-----------|
| **Pureza** | Pode ter mais de uma amostra |
| **DOSN** | Determinação de outras sementes nocivas |
| **Umidade** | Teor de umidade |
| **DT** | Determinação de tetrazólio |

### Dados em Tempo Real
- Sincronização automática entre dispositivos via **Firebase Realtime Database**
- Qualquer alteração feita no celular aparece instantaneamente no notebook e vice-versa
- Dados persistentes na nuvem — nada é perdido ao fechar o navegador

---

## 👥 Responsáveis cadastrados

- Marlisson
- Guilhermino
- Jalmir
- Eduardo

---

## 🛠️ Tecnologias utilizadas

| Tecnologia | Uso |
|------------|-----|
| HTML / CSS / JavaScript | Interface do app |
| Firebase Realtime Database | Banco de dados em tempo real |
| Google Vision API | OCR de leitura de etiquetas |
| GitHub Pages | Hospedagem gratuita |

---

## 📁 Arquivos do repositório

| Arquivo | Descrição |
|---------|-----------|
| `sgm-amostragem.html` | Aplicativo completo |
| `icon.png` | Ícone do app (512x512) |
| `atualizar-github.py` | Script para atualizar o app via terminal |

---

## 🔄 Como atualizar o app

Quando houver uma nova versão do arquivo HTML, rode o script no terminal:

```bash
python atualizar-github.py
```

O script faz o upload automático para o GitHub sem precisar acessar o navegador. Aguarde 1-2 minutos para o GitHub Pages publicar a atualização.

---

## 📱 Como instalar no celular

**Android:**
1. Abra o link no Chrome
2. Menu (⋮) → **"Adicionar à tela inicial"**

**iPhone:**
1. Abra o link no Safari
2. Botão compartilhar → **"Adicionar à Tela de Início"**

---

*Desenvolvido para uso interno — SGM Seeds Laboratório de Análise de Sementes*
