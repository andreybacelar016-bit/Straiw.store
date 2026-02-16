# GUIA DE UPLOAD PARA HOSTINGER - STRAIW.STORE

## Instruções Passo a Passo para Publicar o Site

### PASSO 1: Acessar o Painel da Hostinger

1. Acesse https://www.hostinger.com.br/
2. Faça login com suas credenciais
3. Localize o domínio **straiw.store** no painel
4. Clique em "Gerenciar" ao lado do domínio

### PASSO 2: Acessar o Gerenciador de Arquivos

Existem duas formas principais de fazer upload dos arquivos:

#### OPÇÃO A: Gerenciador de Arquivos (Mais Fácil)

1. No painel da Hostinger, clique em "Gerenciador de Arquivos"
2. Navegue até a pasta **public_html** (esta é a pasta raiz do seu site)
3. Delete qualquer arquivo de exemplo que já esteja lá (como index.html padrão)

#### OPÇÃO B: FTP (Para Usuários Avançados)

1. No painel, localize as credenciais FTP
2. Use um cliente FTP como FileZilla
3. Conecte-se ao servidor usando as credenciais fornecidas
4. Navegue até a pasta **public_html**

### PASSO 3: Fazer Upload dos Arquivos

**IMPORTANTE:** Todos os arquivos devem ser colocados diretamente na pasta **public_html**, não em uma subpasta.

Arquivos que você precisa fazer upload:

```
public_html/
├── index.html
├── moda.html
├── maquiagem.html
├── privacidade.html
├── termos.html
├── logo.png
├── robots.txt
└── sitemap.xml
```

**Como fazer upload:**

1. No Gerenciador de Arquivos, clique em "Upload"
2. Selecione TODOS os arquivos de uma vez (pode selecionar múltiplos arquivos)
3. Aguarde o upload completar (você verá uma barra de progresso)
4. Verifique que todos os 8 arquivos estão na pasta public_html

### PASSO 4: Verificar Permissões

1. Selecione todos os arquivos HTML
2. Clique com botão direito > Permissões (ou "Chmod")
3. Configure para **644** (rw-r--r--)
4. Para a pasta public_html, configure **755** (rwxr-xr-x)

### PASSO 5: Configurar SSL/HTTPS

**CRÍTICO para SEO e Segurança:**

1. No painel da Hostinger, procure por "SSL" ou "Certificado SSL"
2. Ative o SSL gratuito (Let's Encrypt) para straiw.store
3. Aguarde 10-15 minutos para o certificado ser emitido
4. Ative "Forçar HTTPS" para redirecionar automaticamente HTTP para HTTPS

### PASSO 6: Testar o Site

Após o upload, teste o site acessando:

- https://straiw.store/ (página inicial)
- https://straiw.store/moda.html
- https://straiw.store/maquiagem.html
- https://straiw.store/privacidade.html
- https://straiw.store/termos.html

**Verifique:**
- ✅ Todas as páginas carregam corretamente
- ✅ O logo aparece em todas as páginas
- ✅ Links entre páginas funcionam
- ✅ Links de produtos (afiliados) funcionam
- ✅ Site está usando HTTPS (cadeado verde no navegador)

### PASSO 7: Configurar DNS (Se Necessário)

Se o domínio não estiver apontando corretamente:

1. Vá para "Zona DNS" ou "DNS Settings"
2. Verifique que os registros A apontam para o IP do servidor Hostinger
3. Verifique registro CNAME para www
4. Aguarde propagação DNS (pode levar até 24-48 horas, geralmente 1-2 horas)

**Registros DNS típicos:**
```
Tipo    Nome    Aponta Para
A       @       [IP do servidor Hostinger]
CNAME   www     straiw.store
```

### PASSO 8: Submeter aos Mecanismos de Busca

Após o site estar no ar:

1. **Google Search Console**
   - Acesse https://search.google.com/search-console
   - Adicione a propriedade: straiw.store
   - Verifique propriedade (via HTML file upload ou DNS)
   - Submeta o sitemap: https://straiw.store/sitemap.xml

2. **Bing Webmaster Tools**
   - Acesse https://www.bing.com/webmasters
   - Adicione o site
   - Submeta o sitemap

### RESOLUÇÃO DE PROBLEMAS COMUNS

#### Problema: Página mostra erro 404
**Solução:** Verifique que index.html está diretamente em public_html, não em subpasta

#### Problema: Logo não aparece
**Solução:** 
- Verifique que logo.png está em public_html
- Limpe cache do navegador (Ctrl + F5)
- Verifique permissões do arquivo (deve ser 644)

#### Problema: Site não carrega / Erro de conexão
**Solução:**
- Aguarde propagação DNS (até 48h)
- Verifique configurações DNS no painel
- Teste usando IP direto do servidor

#### Problema: HTTPS não funciona
**Solução:**
- Aguarde emissão do certificado SSL (10-15 minutos)
- Force renovação do SSL no painel
- Limpe cache do navegador

#### Problema: Página branca ou erro 500
**Solução:**
- Verifique permissões (644 para arquivos, 755 para pastas)
- Verifique que arquivos não foram corrompidos no upload
- Refaça upload dos arquivos

### MANUTENÇÃO REGULAR

**Semanal:**
- Verificar que todos os links de produtos ainda funcionam
- Backup dos arquivos (Hostinger geralmente faz automaticamente)

**Mensal:**
- Atualizar informações de produtos se necessário
- Verificar certificado SSL está ativo
- Revisar estatísticas no Google Analytics (quando implementado)

### CONTATO HOSTINGER SUPORTE

Se encontrar problemas que não consegue resolver:

- **Chat ao vivo:** Disponível 24/7 no painel da Hostinger
- **Email:** Através do sistema de tickets no painel
- **Base de conhecimento:** https://support.hostinger.com/

---

## CHECKLIST FINAL

Antes de considerar o site oficialmente lançado, confirme:

- [ ] Todos os 8 arquivos foram carregados na pasta public_html
- [ ] Site carrega em https://straiw.store/ com HTTPS (cadeado verde)
- [ ] Todas as 5 páginas (index, moda, maquiagem, privacidade, termos) abrem corretamente
- [ ] Logo aparece em todas as páginas
- [ ] Navegação entre páginas funciona
- [ ] Links de produtos afiliados funcionam e abrem na Amazon/Mercado Livre
- [ ] SSL está ativo e forçado
- [ ] Sitemap foi submetido ao Google Search Console
- [ ] Mobile responsiveness funciona (teste no celular)
- [ ] Você substituiu os links genéricos pelos seus links reais de afiliação

---

**Site pronto para lançamento quando todos os itens do checklist estiverem marcados!**

Qualquer dúvida sobre o processo de upload, consulte a documentação da Hostinger ou entre em contato com o suporte 24/7 deles.
