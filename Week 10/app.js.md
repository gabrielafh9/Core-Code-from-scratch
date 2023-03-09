# app.js

``` Javascript
//===================================================== memory
let memory = [];
let activeOperation = null;
let prevOperation = null;


//===================================================== display
const display = document.querySelector('#display');


//===================================================== ac
const ac = document.querySelector('#ac');

ac.addEventListener('click', () => {
    ac.innerHTML = 'AC';
    display.innerHTML = '0';
});

//===================================================== sig
const sig = document.querySelector('#sig');

sig.addEventListener('click', () => {
    const currentDisplay = display.innerHTML;
    let newDisplay = `${Number(currentDisplay) * -1}`;
    if (currentDisplay === '0'){
        newDisplay = '-0';
    }
    display.innerHTML = newDisplay;
});

//===================================================== percent
const percent = document.querySelector('#percent');

percent.addEventListener('click', () => {
    const currentDisplay = display.innerHTML;
    display.innerHTML = `${Number(currentDisplay) / 100}`;
});

//====================================================== decimal
const dot = document.querySelector('#dot');

const decimalHandler = () => {
    console.log('Hola!');
    const currentDisplay = display.innerHTML;
    if (currentDisplay.indexOf('.') > 0) return;
    display.innerHTML = `${currentDisplay}.`;
};

dot.addEventListener('click', () => decimalHandler());

//====================================================== equal
const equal = document.querySelector('#equal');

const equalHandler = () => {
    // ['58', '*'] ==> 58*
    const operation = `${memory.join(' ')} ${Number(display.innerHTML)}`;
    display.innerHTML = `${eval(operation)}`;
    memory = [];
    activeOperation = null;
    prevOperation = null;
};

equal.addEventListener('click', () => equalHandler());

//====================================================== operators
const div = document.querySelector('#div');
const nul = document.querySelector('#nul');
const sum = document.querySelector('#sum');
const sub = document.querySelector('#sub');

const operators = [ 
    {el: div, op: '/'},
    {el: nul, op: '*'},
    {el: sum, op: '+'},
    {el: sub, op: '-'},
];

//HOVER: 
//background-color:#ffffff;
//color: #ee6c4d;

//NORMAL: 
//background-color: #ee6c4d;
//color: #ffffff;

const setSelectedOperation = (elOp) => {
    elOp.style.backgroundColor = '#ffffff';
    elOp.style.color = '#ee6c4d';
}

const setUnSelectedOperation = (elOp) => {
    elOp.style.backgroundColor = '#ee6c4d';
    elOp.style.color = '#ffffff';
}

const operationHandler = (op, opEl)  => {
    setSelectedOperation(opEl);
    const currentDisplay = display.innerHTML;
    if(memory.length === 0) {
        memory.push(currentDisplay);
    }
    if(memory.length > 1){
        equalHandler();
        memory.push(Number(display.innerHTML));
    }

    memory.push(op);
    activeOperation = opEl;
    prevOperation = opEl;
    console.log(memory)
};

operators.forEach((oper) =>
   oper.el.addEventListener('click', () => operationHandler(oper.op, oper.el))
);

//===================================================== numbers

const zero = document.querySelector('#zero');
const one = document.querySelector('#one');
const two = document.querySelector('#two');
const three = document.querySelector('#three');
const four = document.querySelector('#four');
const five = document.querySelector('#five');
const six = document.querySelector('#six');
const seven = document.querySelector('#seven');
const eight = document.querySelector('#eight');
const nine = document.querySelector('#nine');

const numbers = [zero, one, two, three, four, five, six, seven, eight, nine];

const numberHandler = (n) => {

    if(prevOperation !== null) {
        setUnSelectedOperation(prevOperation);
        display.innerHTML = '';
        activeOperation = null;
    }

    ac.innerHTML = 'C';
    const currentDisplay = display.innerHTML;
    let newDisplay = `${currentDisplay}${n}`;
    if (currentDisplay === '0') {
        newDisplay = n;
    }
    display.innerHTML = `${Number(newDisplay)}`;
};

numbers.forEach((n, i) => n.addEventListener('click', () => numberHandler(i)));
```
