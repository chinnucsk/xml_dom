xml_dom
=======

simiple xml dom parser for erlang

test.xml:

    <a>
        <b c="1" d="2">hello
        </b>
        <c />
    </a>

Parsed result is:

    1> xml_dom:simple_form("test.xml").
    {"a",[],
     [{"b",[{"c","1"},{"d","2"}],"hello\n  "},{"c",[],[]}]}
    2>
