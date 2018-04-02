
Code: https://github.com/lexml/lexml-linker

Entry point: https://github.com/lexml/lexml-linker/blob/master/src/main/haskell/LinkerTool.hs

Chamada ao linker: https://github.com/lexml/lexml-linker/blob/master/src/main/haskell/LinkerTool.hs#L99

Linker: https://github.com/lexml/lexml-linker/blob/master/src/main/haskell/LexML/Linker.hs

Prepara o contexto

    let context = makeContext (loContext lo)

https://github.com/lexml/lexml-linker/blob/5a02bc3d8ac49115ce227c59fd89dd54aadfae06/src/main/haskell/LexML/Linker.hs#L129

    (modMap,logMsgs) = parseReferencias2 logComps (loResolverUrl lo) context tokens (loConstituicaoSimples lo)

ParserReferencias2

https://github.com/lexml/lexml-linker/blob/master/src/main/haskell/LexML/Linker/Parser.hs

Conecta com regras2: https://github.com/lexml/lexml-linker/blob/5a02bc3d8ac49115ce227c59fd89dd54aadfae06/src/main/haskell/LexML/Linker/Parser.hs#L56

Regras2: https://github.com/lexml/lexml-linker/blob/master/src/main/haskell/LexML/Linker/Regras2.hs

checkInitialToken 

    initialWords = S.fromList [
        "lei",
        "leis",
        "decreto",
        "decretos",
        "resolução",
        "resolucao",    
        "resoluções",
        "resolucoes",
        "regulamento",
        "clt",
        "consolidação",
        "consolidacao",
        "constituição",
        "constituicao",
        "projeto",
        "projetos",
        "súmula",
        "sumula",
        "emenda",
        "emendas",
        "medida",
        "medidas",
        "artigo",
        "art",
        "artigos",
        "arts",
        "parágrafo",
        "paragrafo",
        "par",
        "parágrafos",
        "paragrafos",
        "pars",
        "regimento",
        "ato",
        "caput",
        "cpt",
        "inciso",
        "inc",
        "incisos",
        "incs",
        "alínea",
        "alinea",
        "alíneas",
        "alineas",
        "item",
        "itens",
        "letra",
        "letras"
    ]
    