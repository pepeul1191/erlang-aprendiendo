# Erlang

### Instalación Erlang

    $ wget https://packages.erlang-solutions.com/erlang-solutions_1.0_all.deb
    $ sudo dpkg -i erlang-solutions_1.0_all.deb
    $ sudo apt-get update
    $ sudo apt-get install erlang

### Instalación de rebar3:

    $ wget https://s3.amazonaws.com/rebar3/rebar3 && chmod +x rebar3
    $ ./rebar3 local install

Añadir la siguiente variable de entorno 'export PATH=$PATH:~/.cache/rebar3/bin' en

    $ pluma ~/.profile

Cerrar la sesión y volver a entrar

Crear nuevo proyecto con rebar3:

    $ rebar3 new release myrelease
    $ rebar3 compile
    $ rebar3 get-deps

### Ejecutar archivo erlang:

    $ erl
    > pwd(). %% ver la ruta actual
    > ls(). %% ver los archivos de carpeta
    > cd("/home/pepe/Documentos/erlang/aprendiendo").
    > c(tut).
    > tut:hello_world().
    > tut:add(3,4).

10''

---

Fuentes:

+ https://tecadmin.net/install-erlang-on-ubuntu/#
+ https://github.com/erlang/rebar3
+ https://www.youtube.com/watch?v=IEhwc2q1zG4&t=913s
