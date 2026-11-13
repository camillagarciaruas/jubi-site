# Site do Jubí

Site público do aplicativo Jubí, publicado no Cloudflare Pages (jubiapp.com).

- `index.html`: página inicial de divulgação.
- `privacidade/index.html`: política de privacidade, exigida pela App Store,
  pela Google Play e pela verificação do login com Google.
- `assets/`: fotos e ícone (vindos do app).

## Links das lojas

Na `index.html`, procure por `#LINK-GOOGLE-PLAY` e `#LINK-APP-STORE` e troque
pelos links reais quando o app for publicado (cada um aparece duas vezes).

## Política de privacidade

**Não edite `privacidade/index.html` aqui.** Ele é gerado a partir do texto que
está dentro do app, em `app/privacidade.tsx` do repositório principal. Para
atualizar:

```bash
node scripts/gerar-privacidade-web.mjs   # no repositório do app
```

O script já copia o resultado para `privacidade/index.html` quando esta pasta
existe ao lado da pasta do app. Depois é só commitar e dar push aqui; o
Cloudflare publica sozinho.
