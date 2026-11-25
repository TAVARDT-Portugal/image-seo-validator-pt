# Otimizador e Verificador de SEO para Imagens

[![Otimizador Imagens SEO](https://img.shields.io/badge/TAVARDT-Image%20SEO-5b3cf5.svg)](https://tools.tavardt.com/pt/otimizador-imagens-seo/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Auditoria de integridade de texto alternativo, adocao de formatos WebP e AVIF, dimensoes de estabilidade visual e metadados sociais.

***

## Vetores de Risco e Impacto Operacional na Entrega de Imagens

A omissao de texto alternativo cria barreiras diretas de acessibilidade e impede a correta indexacao nos motores de busca em Portugal. Descricoes genericas ou codigos de ficheiro reduzem a relevancia semantica e prejudicam o posicionamento nos resultados.

A distribuicao de formatos pesados sem compressao consome largura de banda excessiva e retarda o carregamento em redes moveis. Nao definir largura e altura explicitas provoca oscilacoes inesperadas de layout e degrada os indicadores de estabilidade visual.

***

## Capacidades Centrais de Auditoria Tecnica

* **Auditoria Critica de Texto Alternativo (Alt)**: Rastreia cada elemento de imagem identificando ausencias de alt, aplicando deducao de ate 35 pontos com alerta critico.
* **Filtragem de Descricoes Genericas**: Detecta termos como imagem, foto e nomes de ficheiros de camara, deduzindo 5 pontos por ocorrencia ate o teto de 15 pontos.
* **Adocao de Formatos de Proxima Geracao**: Avalia a presenca de formatos modernos WebP, AVIF e SVG em relacao a ficheiros legados JPEG e PNG, com penalidade de ate 20 pontos.
* **Prevencao de Deslocamento de Layout (CLS)**: Verifica a existencia de dimensoes explicitas width e height, penalizando elementos sem dimensoes em 3 pontos cada ate 20 pontos.
* **Inspecao de Carregamento Adiado (Lazy Loading)**: Analisa o uso da diretiva loading='lazy' para assegurar a postergacao de imagens fora da primeira dobra.
* **Validacao de Metadados Open Graph**: Avalia a integracao da tag og:image para a geracao de pre-visualizacoes ricas em redes e partilhas, penalizando em 10 pontos a ausencia.
* **Indice de Conformidade de SEO Visual**: Computa pontuacao tecnica de 0 a 100 categorizada em COMPLIANT, WARNING ou CRITICAL.

***

## Instalacao e Execucao

Requer Python 3.8 ou superior utilizando exclusivamente bibliotecas padrao.

```bash
git clone https://github.com/TAVARDT-Portugal/image-seo-validator-pt.git
cd image-seo-validator-pt
python image_seo_scanner.py https://empresa.pt
```

Para gerar a saida em formato estruturado JSON em esteiras de integracao continua:

```bash
python image_seo_scanner.py https://empresa.pt -j
```

***

## Perguntas Frequentes (FAQ Tecnico)

### 1. Qual o impacto da ausencia de atributos alt na indexacao e conformidade de acessibilidade?
Os motores de busca utilizam o texto alternativo para identificar o tema da midia e alimentar a pesquisa visual. A falta do atributo alt infringe diretrizes internacionais de acessibilidade e impede a compreensao por modelos de linguagem.

### 2. Por que a ferramenta penaliza descricoes genericas como nomes de arquivos ou termos vagos?
Palavras como imagem ou codigos de camera nao fornecem nenhuma informacao contextual util para tecnologias assistivas. Os algoritmos de classificacao interpretam essas descricoes como conteudo de baixa qualidade e descartam a pontuacao semantica.

### 3. Como a definicao explicita de dimensoes de imagem previne o Cumulative Layout Shift?
Informar largura e altura explicitas permite que os navegadores reservem o espaco geometrico antes do download do arquivo. A omissao desses parametros provoca rearranjos repentinos de conteudo durante o carregamento e prejudica as notas de Core Web Vitals.

### 4. Quais as vantagens operacionais dos formatos WebP e AVIF sobre JPEG e PNG tradicionais?
Formatos modernos oferecem taxas de compactacao muito superiores, reduzindo o tamanho dos arquivos em ate cinquenta por cento sem degradacao visual. Essa economia acelera a exibicao de conteudo e diminui o consumo de dados em dispositivos moveis.

### 5. Por que a presenca da tag Open Graph para imagens e fundamental na distribuicao de conteudo?
Plataformas digitais e motores de resposta utilizam a tag og:image para construir cartoes visuais durante a analise de URLs. A ausencia desse metadado resulta em links desprovidos de elementos visuais que apresentam taxas de clique sensivelmente menores.

***

## Consultoria em Acessibilidade Visual e Otimizacao de Media

Para portais de grande dimensao e alinhamento com as diretrizes do W3C WCAG, consulte os especialistas em engenharia da **TAVARDT**.

***

## Links Uteis

* **Portal Corporativo:** https://ag.tavardt.com/pt/
* **Suite de Diagnosticos:** https://tools.tavardt.com/pt/
* **Contacto Tecnico:** https://ag.tavardt.com/pt/contacto/

***

### Licenca
Distribuido sob a Licenca MIT. Consulte o arquivo LICENSE para termos completos.

***

© 2026 TAVARDT. Todos os direitos reservados.
