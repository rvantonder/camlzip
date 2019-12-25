all: minizip minigzip testzlib minizip_on_linux

minigzip: ../zip.cma minigzip.ml
	ocamlc -ccopt -g -g -I .. -o minigzip ../zip.cma minigzip.ml

minizip: ../zip.cma minizip.ml
	ocamlc -ccopt -g -g -I .. -o minizip unix.cma ../zip.cma minizip.ml

minizip_on_linux: ../zip.cma minizip_on_linux.ml
	ocamlc -ccopt -g -g -I .. -o minizip_on_linux unix.cma ../zip.cma minizip_on_linux.ml

testzlib: ../zip.cma testzlib.ml
	ocamlc -g -I .. -o testzlib ../zip.cma testzlib.ml

clean:
	rm -f *.cm*
	rm -f minigzip minizip testzlib minizip_on_linux
