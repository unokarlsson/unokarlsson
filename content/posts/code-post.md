+++
title = "Code post"
date = 2018-11-03T12:15:29+01:00
draft = true
categories = ["Programming"]
tags = ["rust","go","java"]

+++

Rust is a modern version of C/C++. Its goal is to be as fast as C/C++ but also add high level abstraction to ease the codeing and robustness.
This is an example of a RUST program.

{{< highlight rust "linenos=table,hl_lines=4-7,linenostart=1" >}}

extern crate rand;
use rand{thread_rng, Rng};

fn read_guess() u8 -> {
    let number: u8 = read();
    number
}

fn main() {
    let number:u8  = thread_rng().gen_range(0,100)+1;
    let mut done   = false;
    while !done {
        let guess = read_guess();
        if guess < number {
            println!("Du gissade för lågt.");
        } else if guess > number {
            println!("Du gissade för högt.");
        } else {
            println!("Du gissade rätt!");
            done = true;
        }
    }
}
{{</highlight>}}

RUST guess number program.

More info about [RUST programming language](https://www.rust-lang.org/sv-SE/)

An example of a GO lang program.

{{<highlight go "linenos=inline,hl_lines=2 3">}}
var a string
var b string
var c string
var d string
{{</highlight>}}

HTML example

{{<highlight html>}}
<section id="main">
  <div>
    <h1 id="title">{{ .Title }}</h1>
    {{ range .Data.Pages }}
      {{ .Render "summary"}}
    {{ end }}
  </div>
</section>
{{</highlight>}}

And some java code:

{{< highlight java "linenos=tabel,linenostart=1">}}
public class Prime {

    public static void main(String[] args) {

        int num = 29;
        boolean flag = false;
        for(int i = 2; i <= num/2; ++i)
        {
            // condition for nonprime number
            if(num % i == 0)
            {
                flag = true;
                break;
            }
        }

        if (!flag)
            System.out.println(num + " is a prime number.");
        else
            System.out.println(num + " is not a prime number.");
    }
}
{{< /highlight >}}

Last highlight example!

Run the command `$ ls -l` to list files in current directory.

