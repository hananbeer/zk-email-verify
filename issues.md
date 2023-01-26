1. there are four different snarkjs versions mentioned in the README; however only this one worked for me:
`yarn add snarkjs@git+https://github.com/vb7401/snarkjs.git#24981febe8826b6ab76ae4d76cf7f9142919d2b8`

2. many paths are comingled and incorrect:
    -  ./circuits/inputs is not created if not exists and causes failure
    - input_twitter.json vs. input_email.json in ./circuits/inputs/
    - keys are created as circuit.zkey{b..k} in ./build/email/ but are later looked at as email.zkey{b..k} in ./build/email

