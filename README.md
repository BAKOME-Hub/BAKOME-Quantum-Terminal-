
<p align="center">
  <img src="https://via.placeholder.com/800x400/0a0a0a/00ff88?text=BAKOME+QUANTUM+TERMINAL+Rust+20K+Lines" alt="BAKOME QUANTUM TERMINAL" width="100%">
</p>

---

## 📖 Description

**🇫🇷 Français**
BAKOME QUANTUM TERMINAL est un terminal de trading quantique écrit en Rust, conçu pour opérer sur les marchés Forex, Crypto, Actions et Prédictifs. Il intègre 10 modules avancés : bridge ultra-rapide vers MetaTrader 5, moteur Order Flow avec analyse du carnet d'ordres en temps réel (delta, spoofing, icebergs), Footprint Charts pour le volume profile, scanner multi-paires surveillant 28 actifs simultanément, IA prédictive basée sur un réseau neuronal LSTM, analyseur de sentiment NLP, matrice de corrélations multi-actifs (XAUUSD vs DXY vs BTC vs SPX), algorithme génétique NSGA-II qui fait évoluer les stratégies automatiquement chaque nuit, et dashboard web intégré. Le tout dans un seul fichier Rust, compilé en un binaire de moins de 10 Mo, qui tourne sur un Pixel 4a 5G. Développé intégralement à Goma, RDC.

**🇬🇧 English**
BAKOME QUANTUM TERMINAL is a quantum trading terminal written in Rust, designed for Forex, Crypto, Stocks and Prediction markets. It features 10 advanced modules: ultra-fast MetaTrader 5 bridge, Order Flow engine with real-time order book analysis (delta, spoofing, icebergs), Footprint Charts, 28-pair scanner, LSTM neural AI, NLP sentiment analyzer, multi-asset correlation matrix (XAUUSD vs DXY vs BTC vs SPX), NSGA-II genetic algorithm that auto-evolves strategies, and integrated web dashboard. Single Rust file, sub-10MB binary, running on a Pixel 4a 5G. Built entirely in Goma, DRC.

**🇪🇸 Español**
BAKOME QUANTUM TERMINAL es un terminal de trading cuántico escrito en Rust, diseñado para Forex, Crypto, Acciones y Mercados Predictivos. Integra 10 módulos avanzados: bridge ultra-rápido a MetaTrader 5, motor Order Flow con análisis del libro de órdenes (delta, spoofing, icebergs), Footprint Charts, escáner de 28 pares, IA neuronal LSTM, analizador de sentimiento NLP, matriz de correlaciones multi-activos (XAUUSD vs DXY vs BTC vs SPX), algoritmo genético NSGA-II que auto-evoluciona estrategias, y dashboard web integrado. Un solo archivo Rust, binario de menos de 10 MB, ejecutándose en un Pixel 4a 5G. Desarrollado íntegramente en Goma, RDC.

---

## ⚡ Modules / Features / Módulos

| Module | Description |
|--------|-------------|
| 🔗 **Bridge Rust ↔ MQL5** | Communication ultra-rapide avec MetaTrader 5 via TCP |
| 📊 **Order Flow + DOM** | Analyse du carnet d'ordres en temps réel (delta, déséquilibres) |
| 🕵️ **Détecteur Spoofing** | Repérage des fausses murailles d'ordres institutionnelles |
| 🧊 **Détecteur Iceberg** | Identification des ordres cachés des grandes mains |
| 👣 **Footprint Charts** | Volume profile par prix, delta acheteur/vendeur, POC |
| 🔍 **Scanner 28 Paires** | Surveillance simultanée Forex, Crypto, Indices |
| 🧠 **IA Prédictive LSTM** | Réseau neuronal pour prédire les mouvements directionnels |
| 📰 **Sentiment NLP** | Analyse des news, tweets, flux Telegram en temps réel |
| 🔗 **Corrélations Multi-Actifs** | Matrice XAUUSD vs DXY vs BTC vs SPX vs VIX |
| 🧬 **Algo Génétique NSGA-II** | Évolution automatique des stratégies chaque nuit |
| 💻 **Dashboard Web** | Interface live intégrée sur le port 8080 |
| 🌍 **Multi-Marchés** | Forex, Crypto (Binance), Actions (IBKR), Prédictifs (Polymarket) |

---

## 🌍 Marchés Supportés

| Marché | Plateformes | Actifs |
|--------|-------------|--------|
| 🪙 **Crypto Spot & Futures** | Binance, Bybit, OKX, Hyperliquid | BTC, ETH, SOL, XAU tokenisé |
| 📈 **Forex & Métaux** | MetaTrader 5 (bridge natif) | XAUUSD, EURUSD, GBPUSD, 28 paires |
| 📊 **Actions & ETFs** | Interactive Brokers, Alpaca | SPX, NASDAQ, actions US |
| 🎯 **Marchés Prédictifs** | Polymarket | Événements réels tokenisés |

---

## ⚙️ Quick Install / Installation rapide

```bash
# 1. Cloner le repo
git clone https://github.com/BAKOME-Hub/BAKOME-Quantum-Terminal.git
cd BAKOME-Quantum-Terminal

# 2. Compiler (Rust requis)
cargo build --release

# 3. Lancer
./target/release/bakome_quantum_terminal

# 4. Dashboard
# Ouvrir http://localhost:8080
