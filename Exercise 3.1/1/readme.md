![Alt text](C:\Users\anees\OneDrive\Pictures\Screenshots 1)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <style>
        h1 {
        text-align: center;
        color: rgb(47, 33, 33);
        }
        h2 {
        text-decoration: underline;
        }
        .highlight {
        background-color: rgb(193, 248, 12);
        font-weight: bold;
        }
        body{
            background-color:rgb(224, 213, 213);
            font-family:Arial, Helvetica, sans-serif;
            font-weight: 700;
            color:black;
        }
        </style>
        </head>
        <body>
        <div style="border: 10px solid rgb(38, 224, 87) ; padding: 15px;">
        </div>
        <h1 style="font-size: 24px; font-weight: bold; font-style: italic;
        background-color: rgb(211, 255, 14); color: rgb(237, 5, 5);">welcome chapter-1</h1>
        <h2>Introduction to Stream Ciphers</h2>
        <p>Cryptography is essential for safeguarding Symmetric cryptography is split into <span class="highlight"> block ciphers and stream ciphers,</span> which
            are easy to distinguish.
            Figure i below shows the operational differences between stream and block
            ciphers when we want to encrypt b bits at a time, where b is the width of the
            block cipher </p>
        <h2>Random Number Generators</h2>
        <ul>
            <li>True Random Number Generators</li>
            <li>Pseudorandom Number Generators</li>
            <li>Cryptographically Secure Pseudorandom Number Generators</li>
        </ul>
        <p><h2> True Random Number Generators (TRNG) :</h2>True random number generators (TRNGs) are characterized by the fact that
            their output cannot be reproduced. For instance, if we flip a coin 100 times
            and record the resulting sequence of 100 bits, it will be virtually impossible
            for anyone on Earth to generate the same 100 bit sequence. <span class="highlight"> chance of
            success is (1/2)</span>
            100, which is an extremely small probability. TRNGs are based
            on physical processes.
            Examples include coin flipping, rolling of dice</p>
        <p><h2>Pseudorandom Number Generators (PRNG) : </h2>
            Pseudo-random number generators (PRNGs) are algorithms used to produce
            sequences of numbers that approximate the properties of random numbers.
            Unlike true random numbers, which are generated from physical processes (like
            radioactive decay or thermal noise), pseudo-random numbers are produced
            using deterministic processes. This means that <span class="highlight"> you know the initial state
            (often called the "seed") and the algorithm, you can predict the entire sequence
            of numbers</span></p>
        <p><h2>Cryptographically Secure Pseudorandom Number Generators (CSPRNG) :</h2>Cryptographically secure pseudorandom number generators (CSPRNGs) are
            a special type of PRNG which possess the following additional property: A CSPRNG is PRNG which is unpredictable. Informally, this means that given n output bits of <span class="highlight">key stream si
            , si+1, . . . , si+n1,</span> where n is some integer, it is
            computationally infeasible to compute the subsequent bits si+n, si+n+1, . . . . A
            more exact definition is that given n consecutive bits of the key stream,<span class="highlight" >there
            is no polynomial time algorithm that can predict the next bit sn + 1 with
            better than 50% chance of success.</span> Another property of CSPRNG is that
            given the above sequence, it should be computationally infeasible to compute
            any preceding bits si1, si2, . . . .</p>
</body>
</html>
