# voa-plugin-dist

Repositório público para disponibilização do script do **plugin Voa** (`plugin.js`) para colocar no seu prontuário ou sistema web.

> Caso precise reportar erros ou solicitar features entre em contato com o suporte: https://crm.voa.health/enterprise

---

## O que tem neste repositório?


| Arquivo      | O que é                                      |
| ------------ | -------------------------------------------- |
| `plugin.js`  | Plugin Voa compilado, pronto para `<script>` |

Cada **release** (tag `vX.Y.Z`) traz uma versão nova desse arquivo. A página de [Releases](https://github.com/Voa-Health/voa-plugin-dist/releases) funciona como **changelog público** do plugin.

---

## Como usar (jsDelivr)

O jeito mais simples é carregar o script pelo [jsDelivr](https://www.jsdelivr.com/), um CDN gratuito que serve arquivos do GitHub.

### Recomendado: `@latest` (sempre a versão mais recente)

É recomendado que utilize sempre que possível a versão `@latest` para receber automaticamente correções e novas funcionalidades.

```html
<script src="https://cdn.jsdelivr.net/gh/Voa-Health/voa-plugin-dist@latest/plugin.js"></script>
```

> O jsDelivr pode cachear `@latest` por algumas horas.

### Versão fixa (`@vX.Y.Z`)

Caso precise, você também pode apontar para uma versão específica.
Neste caso, lembre-se de acompanhar nossa página de [Releases](https://github.com/Voa-Health/voa-plugin-dist/releases) para manter sua versão atualizada.

```html
<script src="https://cdn.jsdelivr.net/gh/Voa-Health/voa-plugin-dist@v2.4.0/plugin.js"></script>
```

Troque `v2.4.0` pela versão desejada e disponível em uma tag que exista na [página de Releases](https://github.com/Voa-Health/voa-plugin-dist/releases).

Para manter atualizado automaticamente, prefira utilizar a versão `@latest`.

---

## Passo a passo

1. **Copie** a linha `<script>` acima (`@latest`) para o HTML do seu sistema (ou template do EHR), antes do `</body>` ou onde sua equipe costuma colocar scripts de terceiros.
2. **Implemente sua integração** segundo a [documentação do plugin](https://docs.voa.health/integracao/plugin).
3. **Abra o prontuário** no navegador e confira se o plugin Voa aparece (barra/flutuante conforme a integração).
4. Se algo quebrar, abra o **Console** do navegador (F12 → Console) e veja erros de rede ou JavaScript.
5. Para documentação completa (eventos, configuração, etc.), use [docs.voa.health](https://docs.voa.health) (seção "plugin").

---

## Perguntas frequentes

### Preciso clonar este repositório?

Não. Basta usar a URL do jsDelivr no seu HTML.

### Onde vejo o que mudou em cada versão?

[Releases do voa-plugin-dist](https://github.com/Voa-Health/voa-plugin-dist/releases).

### Como conseguir suporte?

Para suporte, fale o suporte acordado no seu contrato ou em https://crm.voa.health/enterprise.

---

## Licença e suporte

Distribuição fornecida pela [Voa Health](https://voa.health).
Para suporte acesse: https://crm.voa.health/enterprise
