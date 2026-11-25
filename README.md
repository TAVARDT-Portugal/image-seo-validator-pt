# Otimizador e Verificador de SEO para Imagens

[![Otimizador Imagens SEO](https://img.shields.io/badge/TAVARDT-Image%20SEO-5b3cf5.svg)](https://tools.tavardt.com/pt/otimizador-imagens-seo/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)](https://www.python.org/)

Inspeção tecnica de etiquetas alt, formatos de ultima geracao e estabilidade visual sob recomendacoes W3C.

Desenvolvido e mantido pela divisao de arquitetura web e acessibilidade da **TAVARDT Portugal**.

***

## Capacidades de Auditoria de SEO para Imagens

* **Inspeção de Textos Alternativos Alt**: Avaliacao rigorosa da presenca e relevancia dos atributos `alt` em todas as imagens.
* **Formatos de Nova Geracao**: Identificacao da adocao de formatos de alto rendimento (WebP e AVIF).
* **Mitigacao de Instabilidade de Layout (CLS)**: Confirmacao da definicao de dimensoes `width` e `height` nos elementos visuais.
* **Carregamento Diferido (Lazy Loading)**: Análise de diretivas `loading="lazy"` para poupanca de largura de banda.
* **Indice de Desempenho Visual**: Metrica quantitativa de 0 a 100 com recomendacoes de otimizacao.

***

## Instalação e Execucao

Requer Python 3.8 ou superior, operando exclusivamente com a biblioteca padrao.

```bash
git clone https://github.com/TAVARDT-Portugal/image-seo-validator-pt.git
cd image-seo-validator-pt
python image_seo_validator.py https://empresa.pt
```

Para inspeção com saída estruturada em JSON:

```bash
python image_seo_validator.py https://empresa.pt -json
```

***

## Diagnostico Completo na Web

Para análise aprofundada de recursos de imagem:

* **Otimizador de Imagens SEO Oficial**
* **[Portal Corporativo TAVARDT](https://ag.tavardt.com/pt/)**

***

## Consultoria em Acessibilidade e Otimizacao Visual

Para auditorias de imagem e conformidade com Normas Europeias de Acessibilidade Web e W3C, consulte a equipa da **TAVARDT Portugal**.

## Links Úteis

* **Portal Corporativo:** https://ag.tavardt.com/pt/
* **Suíte de Diagnósticos:** https://tools.tavardt.com/pt/
* **Contacto Técnico:** https://ag.tavardt.com/pt/contacto/

***

### Licença
Distribuído sob a Licença MIT. Consulte o arquivo [LICENSE](LICENSE) para obter detalhes completos.

***

© 2026 TAVARDT Portugal. Todos os direitos reservados. Soberania e Defesa de Infraestrutura.
