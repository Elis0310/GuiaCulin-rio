# 📓 Diário de Debugging - Guia Culinário

Este arquivo registra os desafios técnicos que encontrei durante o desenvolvimento e as soluções aplicadas.

---

### 🐞 Erro 1: Imagem de capa não aparecia no WhatsApp
* **Problema:** Ao compartilhar o link, a miniatura (og:image) ficava em branco.
* **Causa:** O arquivo continha acentos (`capa-guia-culinário.jpg`) e o link no HTML estava com o nome do usuário em letras minúsculas (`elisa0310`), divergindo do GitHub (`Elis0310`).
* **Solução:** 1. Renomeei o arquivo para `capa-guia-culinario.jpg` usando `git mv`.
    2. Ajustei as metatags para respeitar o *Case Sensitivity* (letras maiúsculas/minúsculas).
    3. Usei parâmetros na URL (`?v=1`) para limpar o cache do WhatsApp.

### 📝 Notas de Git
* **U (Untracked):** Arquivo novo que o Git ainda não conhece.
* **M (Modified):** Arquivo que já existia mas foi alterado.
* **Commit & Push:** O commit salva localmente, o push envia para a "Fonte Única da Verdade" (GitHub).