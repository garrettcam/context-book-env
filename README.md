# context-book-env
Environment file for typesetting books in ConTeXt mkiv

## Sample main file
```
% !TEX TS-program = ConTeXt (LuaTeX)
% !TEX encoding = UTF-8

% ENVIRONMENT & SETTINGS
\enablemode[print] % screen or print
\enablemode[11]		% font size pt [12, 11, 10]
\enablemode[crimson] % font name [crimson, minion, calluna, cormorant]
\environment[env.tex]
\pdftitle{Title}{Author}

%
% START OF ACTUAL DOCUMENT
%
\starttext

\startfrontmatter

  \dosetups[title]
  \dosetups[imprint]
  \dosetups[dedication]

\startbodymatter
	\resetnumber[userpage]

\stopbodymatter

\page[quadruple]
\stoptext
```
