# Smart_Contracts

Реализованы 2 смарт контракта на языке Solidity(Agent и Store).
Функционал контракта Agent: контракт принимает денежные средства (msg.value) и передает их на контракт Store.
Отправитель указывает адрес аккаунта для которого предназначены деньги, таким образом средства может получить адресат, указанный
отправителем, либо сам отправитель, если адресат не забрал деньги.
Функционал контракта Store: принимает на хранение деньги и возвращает их на контракт Agent по запросу. Для отправки средств на контракт Agent Store вызывает функцию из контракта Agent, поэтому никакой иной контракт не может получить деньги со Store.
Реализовано в Remix IDE.
