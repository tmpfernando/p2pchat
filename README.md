# 🗣️ P2P Link

Uma aplicação web direta via navegador (**Peer-to-Peer / WebRTC**) para chamadas de voz, compartilhamento de tela, câmera, chat e envio de arquivos — feita para funcionar sem depender de plataformas pesadas ou bloqueadas.

> ✨ **Vibe Coded com Gemini:** Este projeto foi construído de forma iterativa e *vibe coded* por meio do **Gemini**, nascendo da necessidade prática de ter um recurso rápido e funcional para **compartilhar tela, conversar por voz e trocar arquivos** quando outros sistemas não estão disponíveis ou não são práticos no momento.

---

## 🚀 Por que o P2P Link existe?

Às vezes você só precisa abrir a tela para alguém, falar rápido no microfone ou mandar um arquivo direto — sem instalar cliente, sem criar conta e sem esbarrar em restrições de outros programas. O **P2P Link** resolve isso direto no browser usando **PeerJS / WebRTC**, com **aprovação de entrada pelo criador da sala** e **visualização sob demanda** (telas e câmeras só abrem quando você clica em **Assistir**).

---

## ✨ Destaques

* 🖥️ **Compartilhamento de Tela & Câmera sob demanda:** Transmissão via `getDisplayMedia` / `getUserMedia`, com botão **Assistir** para não abrir janelas de vídeo à força e suporte a **Picture-in-Picture (PiP)**.
* 🎙️ **Áudio com Filtro Vocal & Detecção:** Suporte a detecção automática de voz (com *threshold* e *hold* ajustáveis) ou **Push-to-Talk**, filtros *high-pass* / *low-pass* e controle de volume individual por participante.
* 🔒 **Controle da Sala:** O criador aprova ou recusa pedidos de entrada e pode gerar link direto (`?sala=...`).
* 💬 **Chat & Transferência P2P:** Mensagens de texto, indicador de digitação e envio de arquivos em blocos diretamente entre os pares, com histórico salvo localmente no navegador.
* 🌈 **Temas Escuro, Claro e RGB Super Enfeitado:** Alternância instantânea entre modo escuro, claro e o modo **RGB** com fundo aurora animado, bordas prismáticas pulsantes e botões com gradiente colorido.

---

## 📦 Como publicar no GitHub Pages

1. Crie um repositório no GitHub e salve o código da aplicação como **`index.html`** na raiz.
2. Acesse **Settings → Pages** no repositório.
3. Em **Build and deployment**, selecione a branch (`main`) e a pasta `/ (root)`, depois clique em **Save**.
4. Abra `https://<seu-usuario>.github.io/<seu-repositorio>/` em um navegador moderno (Chrome, Edge, Firefox ou Brave).

---

## 🛠️ Tecnologias

* **HTML5, CSS3 e JavaScript puro** (arquivo único)
* **PeerJS** (`1.5.4`) sobre **WebRTC**
* **Web Audio API** (filtros, medidor de nível, ducking de áudio de tela e detecção de fala)
* **GitHub Pages** para hospedagem estática gratuita

---

## ⚠️ Observações de uso

* Como utiliza **WebRTC** e captura de mídia (`getUserMedia` / `getDisplayMedia`), o acesso exige contexto seguro (**HTTPS**, como no GitHub Pages, ou `localhost`).
* Em algumas redes corporativas ou firewalls mais rígidos, conexões P2P podem sofrer restrições de NAT/rede.
