all:
	ocamlyacc calc.mly
	ocamlc -c calc.mli
	ocamllex lexer.mll
	ocamlc -c lexer.ml
	ocamlc -c calc.ml
	ocamlc -c main.ml
	ocamlc -o calc lexer.cmo calc.cmo main.cmo

repl:
	./calc

test:
	./calc test.ca
