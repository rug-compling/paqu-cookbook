# Introduction

## Lassy

See: [Lassy Syntactische Annotatie](http://www.let.rug.nl/vannoord/Lassy/sa-man_lassy.pdf)

See: [alpino_ds.dtd](https://github.com/rug-compling/Alpino/blob/master/Treebank/alpino_ds.dtd)

## Universal Dependencies

> Het stormt en regent.

```xml
<?xml version="1.0"?>
<alpino_ds version="1.10">

  <node begin="0" end="5" id="0" rel="top" cat="top">
    <node begin="0" end="4" id="1" rel="--" cat="conj">
      <node begin="0" end="2" id="2" rel="cnj" cat="smain">
        <node begin="0" end="1" id="3" index="1" lemma="het"
              postag="VNW(pers,pron,stan,red,3,ev,onz)" pt="vnw" rel="su"
              word="Het" frame="het_noun" genus="onz" getal="ev" his="normal"
              his_1="decap" his_1_1="normal" lcat="np" naamval="stan"
              pdtype="pron" persoon="3" pos="noun" rnum="sg" root="het"
              sense="het" special="het" status="red" vwtype="pers">
          <ud id="1" form="Het" lemma="het" upos="PRON" Person="3"
              PronType="Prs" head="2" deprel="expl" deprel_main="expl">
            <dep id="1" head="2" deprel="expl" deprel_main="expl"/>
            <dep id="1" head="4" deprel="nsubj" deprel_main="nsubj"/>
          </ud>
        </node>
        <node begin="1" end="2" id="4" lemma="stormen" postag="WW(pv,tgw,met-t)"
              pt="ww" rel="hd" word="stormt" frame="verb(hebben,sg3,het_subj)"
              his="normal" his_1="normal" infl="sg3" lcat="smain" pos="verb"
              pvagr="met-t" pvtijd="tgw" root="storm" sc="het_subj"
              sense="het-storm" tense="present" wvorm="pv">
          <ud id="2" form="stormt" lemma="stormen" upos="VERB" Number="Sing"
              Tense="Pres" VerbForm="Fin" head="0" deprel="root"
              deprel_main="root">
            <dep id="2" head="0" deprel="root" deprel_main="root"/>
          </ud>
        </node>
      </node>
      <node begin="2" end="3" id="5" lemma="en" postag="VG(neven)" pt="vg"
            rel="crd" word="en" conjtype="neven" frame="conj(en)" his="normal"
            his_1="normal" lcat="vg" pos="vg" root="en" sense="en">
        <ud id="3" form="en" lemma="en" upos="CCONJ" head="4" deprel="cc"
            deprel_main="cc">
          <dep id="3" head="4" deprel="cc" deprel_main="cc"/>
        </ud>
      </node>
      <node begin="0" end="4" id="6" rel="cnj" cat="ssub">
        <node begin="0" end="1" id="7" index="1" rel="su"/>
        <node begin="3" end="4" id="8" lemma="regenen" postag="WW(pv,tgw,met-t)"
              pt="ww" rel="hd" word="regent" frame="verb(hebben,sg3,het_subj)"
              his="normal" his_1="normal" infl="sg3" lcat="ssub" pos="verb"
              pvagr="met-t" pvtijd="tgw" root="regen" sc="het_subj"
              sense="het-regen" tense="present" wvorm="pv">
          <ud id="4" form="regent" lemma="regenen" upos="VERB" Number="Sing"
              Tense="Pres" VerbForm="Fin" head="2" deprel="conj" deprel_main="conj">
            <dep id="4" head="2" deprel="conj:en" deprel_main="conj"
                 deprel_aux="en"/>
          </ud>
        </node>
      </node>
    </node>
    <node begin="4" end="5" id="9" lemma="." postag="LET()" pt="let" rel="--"
          word="." frame="punct(punt)" his="normal" his_1="normal" lcat="punct"
          pos="punct" root="." sense="." special="punt">
      <ud id="5" form="." lemma="." upos="PUNCT" head="2" deprel="punct"
          deprel_main="punct">
        <dep id="5" head="2" deprel="punct" deprel_main="punct"/>
      </ud>
    </node>
  </node>

  <sentence sentid="0000/0000">Het stormt en regent .</sentence>

  <root ud="basic" id="2" form="stormt" lemma="stormen" upos="VERB"
        Number="Sing" Tense="Pres" VerbForm="Fin" head="0" deprel="root" pt="ww"
        pvagr="met-t" pvtijd="tgw" wvorm="pv">
    <expl ud="basic" id="1" form="Het" lemma="het" upos="PRON" Person="3"
          PronType="Prs" head="2" deprel="expl" genus="onz" getal="ev"
          naamval="stan" pdtype="pron" persoon="3" pt="vnw" status="red"
          vwtype="pers"/>
    <conj ud="basic" id="4" form="regent" lemma="regenen" upos="VERB"
          Number="Sing" Tense="Pres" VerbForm="Fin" head="2" deprel="conj"
          pt="ww" pvagr="met-t" pvtijd="tgw" wvorm="pv">
      <cc ud="basic" id="3" form="en" lemma="en" upos="CCONJ" head="4"
          deprel="cc" conjtype="neven" pt="vg"/>
    </conj>
    <punct ud="basic" id="5" form="." lemma="." upos="PUNCT" head="2"
           deprel="punct" pt="let"/>
  </root>

  <root ud="enhanced" id="2" form="stormt" lemma="stormen" upos="VERB"
        Number="Sing" Tense="Pres" VerbForm="Fin" head="0" deprel="root" pt="ww"
        pvagr="met-t" pvtijd="tgw" wvorm="pv">
    <expl ud="enhanced" id="1" form="Het" lemma="het" upos="PRON" Person="3"
          PronType="Prs" head="2" deprel="expl" genus="onz" getal="ev"
          naamval="stan" pdtype="pron" persoon="3" pt="vnw" status="red"
          vwtype="pers"/>
    <conj ud="enhanced" id="4" form="regent" lemma="regenen" upos="VERB"
          Number="Sing" Tense="Pres" VerbForm="Fin" head="2" deprel="conj:en"
          deprel_aux="en" pt="ww" pvagr="met-t" pvtijd="tgw" wvorm="pv">
      <nsubj ud="enhanced" id="1" form="Het" lemma="het" upos="PRON" Person="3"
             PronType="Prs" head="4" deprel="nsubj" genus="onz" getal="ev"
             naamval="stan" pdtype="pron" persoon="3" pt="vnw" status="red"
             vwtype="pers"/>
      <cc ud="enhanced" id="3" form="en" lemma="en" upos="CCONJ" head="4"
          deprel="cc" conjtype="neven" pt="vg"/>
    </conj>
    <punct ud="enhanced" id="5" form="." lemma="." upos="PUNCT" head="2"
           deprel="punct" pt="let"/>
  </root>

  <conllu status="OK"><![CDATA[
1  Het     het      PRON   VNW|pers|pron|stan|red|3|ev|onz  Person=3|PronType=Prs                2  expl   2:expl|4:nsubj  _
2  stormt  stormen  VERB   WW|pv|tgw|met-t                  Number=Sing|Tense=Pres|VerbForm=Fin  0  root   0:root          _
3  en      en       CCONJ  VG|neven                         _                                    4  cc     4:cc            _
4  regent  regenen  VERB   WW|pv|tgw|met-t                  Number=Sing|Tense=Pres|VerbForm=Fin  2  conj   2:conj:en       _
5  .       .        PUNCT  LET                              _                                    2  punct  2:punct         _
]]></conllu>

</alpino_ds>
```

![boom](storm-regen-tree.png)

![UD](storm-regen-ud.png)

![EUD](storm-regen-eud.png)
