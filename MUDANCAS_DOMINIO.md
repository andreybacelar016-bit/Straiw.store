# MUDANÇAS REALIZADAS PARA O DOMÍNIO STRAIW.STORE

## Arquivos Atualizados

Todos os arquivos foram atualizados para refletir seu novo domínio **straiw.store** hospedado na Hostinger.

### 1. index.html
**Alteração:** Canonical URL atualizada
- **Antes:** `<link rel="canonical" href="https://andreybacelar016.github.io/">`
- **Depois:** `<link rel="canonical" href="https://straiw.store/">`

**Nota:** As meta tags Open Graph e Twitter já estavam com o domínio correto.

### 2. sitemap.xml
**Alteração:** Todas as URLs atualizadas para o novo domínio

**URLs antigas (GitHub):**
```xml
<loc>https://andreybacelar016.github.io/</loc>
<loc>https://andreybacelar016.github.io/moda.html</loc>
etc.
```

**URLs novas (Hostinger):**
```xml
<loc>https://straiw.store/</loc>
<loc>https://straiw.store/moda.html</loc>
<loc>https://straiw.store/maquiagem.html</loc>
<loc>https://straiw.store/privacidade.html</loc>
<loc>https://straiw.store/termos.html</loc>
```

### 3. robots.txt
**Alteração:** Referência ao sitemap atualizada
- **Antes:** `Sitemap: https://andreybacelar016.github.io/sitemap.xml`
- **Depois:** `Sitemap: https://straiw.store/sitemap.xml`

Também atualizado o comentário no topo do arquivo para refletir o novo domínio.

### 4. termos.html
**Alteração:** Referência ao domínio no texto legal
- **Antes:** "...site Straw Urban (andreybacelar016.github.io)..."
- **Depois:** "...site Straw Urban (straiw.store)..."

### 5. Demais arquivos
Os seguintes arquivos não necessitaram alterações pois não continham referências ao domínio:
- moda.html
- maquiagem.html
- privacidade.html
- logo.png
- README.md

---

## Diferenças: GitHub Pages vs Hostinger

### GitHub Pages (domínio antigo)
- **Domínio:** andreybacelar016.github.io
- **Hospedagem:** Gratuita via GitHub
- **Upload:** Via Git (push para repositório)
- **SSL:** Automático e gratuito
- **Limitações:** Apenas sites estáticos

### Hostinger (domínio atual)
- **Domínio:** straiw.store (domínio personalizado)
- **Hospedagem:** Paga via Hostinger
- **Upload:** Via FTP ou Gerenciador de Arquivos
- **SSL:** Let's Encrypt gratuito (precisa ativar)
- **Vantagens:** Mais controle, domínio profissional, suporte 24/7

---

## Impacto SEO da Mudança de Domínio

### Ações Necessárias para Manter SEO

1. **301 Redirects (Se GitHub Pages ainda ativo)**
   - Se o site antigo ainda existir, configure redirects 301 para o novo domínio
   - Isso preserva qualquer autoridade de domínio existente

2. **Atualizar Google Search Console**
   - Adicione o novo domínio straiw.store como nova propriedade
   - Submeta o novo sitemap: https://straiw.store/sitemap.xml
   - Se tinha o domínio antigo verificado, mantenha ambos temporariamente

3. **Atualizar Bing Webmaster Tools**
   - Adicione straiw.store
   - Submeta o novo sitemap

4. **Atualizar Links Externos**
   - Se você compartilhou o site em redes sociais, atualize os links
   - Se tem backlinks apontando para o domínio antigo, entre em contato pedindo atualização

### Timeline Esperada

- **Imediato:** Site acessível no novo domínio
- **24-48h:** DNS totalmente propagado globalmente
- **1-2 semanas:** Google começa a indexar novo domínio
- **2-4 semanas:** Transferência completa de autoridade (se havia site anterior)

---

## Checklist de Verificação Pós-Upload

Após fazer upload dos arquivos na Hostinger, verifique:

### Técnico
- [ ] Site carrega em https://straiw.store/ (com HTTPS, cadeado verde)
- [ ] Todas as páginas carregam sem erros 404
- [ ] Logo aparece corretamente em todas as páginas
- [ ] Navegação entre páginas funciona
- [ ] Links de produtos afiliados abrem corretamente
- [ ] Site é responsivo no mobile (teste no celular)

### SEO
- [ ] robots.txt acessível em https://straiw.store/robots.txt
- [ ] sitemap.xml acessível em https://straiw.store/sitemap.xml
- [ ] Sitemap submetido no Google Search Console
- [ ] Certificado SSL ativo e válido
- [ ] Forçar HTTPS está ativado (redireciona HTTP para HTTPS)

### Conteúdo
- [ ] Todos os textos aparecem corretamente (sem caracteres quebrados)
- [ ] Imagens carregam rapidamente
- [ ] Formulário de newsletter funciona (se implementado)
- [ ] Footer mostra informações corretas

---

## Configurações Recomendadas na Hostinger

### 1. Performance
- Ative cache do servidor (se disponível)
- Ative compressão Gzip/Brotli
- Configure CDN se disponível no seu plano

### 2. Segurança
- Ative SSL e force HTTPS
- Configure backups automáticos
- Ative proteção contra DDoS (se disponível)

### 3. Email Profissional (Opcional mas Recomendado)
Se seu plano Hostinger incluir, crie emails profissionais:
- contato@straiw.store
- suporte@straiw.store
- legal@straiw.store

Atualize os emails de contato em privacidade.html e termos.html quando tiver emails funcionando.

---

## Próximos Passos Após Upload

1. **Imediato (Hoje)**
   - Faça upload de todos os arquivos
   - Ative SSL
   - Teste todas as páginas

2. **Nas Primeiras 24 Horas**
   - Submeta sitemap ao Google Search Console
   - Teste o site em diferentes dispositivos e navegadores
   - Compartilhe o link nas suas redes sociais

3. **Na Primeira Semana**
   - Monitore erros no Google Search Console
   - Configure Google Analytics (se ainda não fez)
   - Comece a divulgar o site

4. **No Primeiro Mês**
   - Adicione mais produtos aos links genéricos
   - Colete feedback de visitantes
   - Otimize baseado em comportamento real dos usuários

---

**Seu site está pronto para ser publicado no novo domínio straiw.store!**

Consulte o arquivo GUIA_UPLOAD_HOSTINGER.md para instruções detalhadas passo a passo de como fazer o upload dos arquivos.
