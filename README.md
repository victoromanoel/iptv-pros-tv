# 🎬 IPTV Pro — Android TV APK

APK para Android TV que carrega o **IPTV Pro Player** em WebView de tela cheia.

## 📺 Recursos
- Tela cheia sem barras de sistema
- Suporte a controle remoto (D-pad) e botão Voltar
- Aparece no launcher do Android TV
- JavaScript, localStorage e reprodução de mídia habilitados
- Tela sempre ligada durante uso

## 🚀 Build automático via GitHub Actions

Toda vez que você fizer **push** na branch `main`, o GitHub Actions:
1. Compila o APK automaticamente
2. Disponibiliza para download na aba **Actions → Artifacts**

### Como baixar o APK após o build:
1. Acesse seu repositório no GitHub
2. Clique na aba **Actions**
3. Clique no último workflow executado
4. Role para baixo até **Artifacts**
5. Baixe `IPTV-Pro-TV-debug`

## 📦 Criar Release com tag

```bash
git tag v1.0.0
git push origin v1.0.0
```

O APK será publicado automaticamente como **GitHub Release**.

## 🔑 Assinar o APK (opcional)

Para assinar o release, configure estes **Secrets** no GitHub (Settings → Secrets → Actions):

| Secret | Descrição |
|--------|-----------|
| `KEYSTORE_BASE64` | Keystore em Base64: `base64 keystore.jks` |
| `KEY_STORE_PASSWORD` | Senha do keystore |
| `KEY_ALIAS` | Alias da chave |
| `KEY_PASSWORD` | Senha da chave |

## 📥 Instalar no Android TV

1. No Android TV: **Configurações → Preferências do dispositivo → Segurança → Apps desconhecidos**
2. Transfira o APK via USB ou use o app **Downloader** (código no AFTV: `https://seu-link`)
3. Instale o APK
