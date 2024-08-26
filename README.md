# FIRST WORK
transaction id
at1ygzyp98l3e3cdvksday3tprtryml0ug3yl8dnnkr743nnuxhes8qs4cfpq!
![overall deployed](https://github.com/user-attachments/assets/86e2a36a-a1db-4d37-a85b-6f9836702e41)
DESCRIPTION
program helloworld_6qkbue4.aleo;

function main:
    input r0 as u32.public;
    input r1 as u32.private;
    add r0 r1 into r2;
    output r2 as u32.private;

#SECOND WORK
transaction Id 
at1ygzyp98l3e3cdvksday3tprtryml0ug3yl8dnnkr743nnuxhes8qs4cfpq!
program simple_token_6k6luju.aleo;

record Token:
    owner as address.private;
    amount as u64.private;

function mint:
    input r0 as address.private;
    input r1 as u64.private;
    cast r0 r1 into r2 as Token.record;
    output r2 as Token.record;

function transfer:
    input r0 as Token.record;
    input r1 as address.private;
    input r2 as u64.private;
    sub r0.amount r2 into r3;
    cast r0.owner r3 into r4 as Token.record;
    cast r1 r2 into r5 as Token.record;
    output r4 as Token.record;
    output r5 as Token.record;
