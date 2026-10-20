# Compressor de PDFs em lote (PowerShell + Ghostscript)

Script que comprime automaticamente todos os PDFs de uma pasta, mantendo
a qualidade do documento e o nome original dos arquivos.

## Problema
No fechamento mensal de faturamento, dezenas de PDFs precisam ser enviados
para portais com limite rígido de tamanho. A compressão era feita manualmente,
lote por lote, em sites online, o que consumia tempo e reduzia a qualidade.

## Solução
1. Identifica os PDFs da pasta informada
2. Cria automaticamente a pasta "Comprimidos"
3. Comprime todos os arquivos com Ghostscript
4. Mantém o nome original e preserva os arquivos originais

## Resultado
- 62 lotes processados em um único fechamento
- Arquivos de 85 MB reduzidos para 15 MB (~82% de redução)
- Qualidade visual praticamente idêntica ao original
- ~20% do tempo do setor devolvido para conferência e análise

## Como usar
1. Instale o [Ghostscript](https://ghostscript.com/releases/gsdnld.html)
2. Baixe o script `compress-pdfs.ps1`
3. Edite a variável da pasta de origem
4. Execute no PowerShell: `.\compress-pdfs.ps1`

## Tecnologias
PowerShell · Ghostscript

## Próximos passos
- Opção para excluir originais após a compressão
- Relatório com tamanho antes/depois por arquivo (CSV)

## Autora
Isabele Rodrigues · [LinkedIn](https://www.linkedin.com/in/isabelerodrigues-dados)
