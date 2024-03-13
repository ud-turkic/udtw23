## sent_id = 2

- parataxis relation of sencond part
	- can't be ccomp because it doesn't act like an object
	- if there were деп, деп would be advcl, сөз кылба would be ccomp of деп
	- without деп, and without explicit object of айтам (like муну), then сөз кылба is ccomp

## sent_id = 3

- (dat+) буюртма <- берген obj vs. compound/compound:lvc
	- See https://github.com/UniversalDependencies/docs/issues/1013
	- There is some evidence of not fully `obj`-like behaviour for indefinite N + V constructions: they can't be made definite, they don't seem to like determiners on the noun, they don't like to inflect, they resist adverbs intervening, etc.
	- There is some evidence that they're `obj`: can kind of take numbers?, can be passivised: _тамакка буютма берилди_, can be extracted in (passive) relative clause: _тамакка берилген буюртма_
	- if we say `obj:lvc` or `compound(:lvc)`, then _пиццага_ would be `obj` (with _баш тарт_, _иштен_ would be `obj`) - we don't want this
	- if we say `obj`, then _пиццага_ is `obl` (with _баш тарт_, _иштен_ would be `obl`) - this is preferable
	- since there's evidence for both compound and `obj`, then we could say `compound:obj`
	- _сөз кылба_ (`sent_id = 2`) is different: no passivisation is possible, no relativisation is possible
	- In Turkish, _yemeğe edilen sipariş_ is not allowed, and _yemeğe sipariş edildi_ is not good either, but _yemek sipariş edildi_ and _yemeği sipariş etti_ are - this is a real LVC, because _sipariş_ is never separated from _et-_, and there is a separate object that becomes subject upon passivisation
	- In Kyrgyz _пиццаны заказ кылдым_ / _пицца заказ кылынды_ work, but _пиццаны кылынган заказ_ doesn't work (all work with _пиццага_) — then _заказ кыл-_ (with accusative) is real LVC; _заказ кыл-_ (with dative) is like _буютма бер-_
	- `compound:obj` works for now for _буютма бер-_

