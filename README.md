# minigrep

This application requires rust to run (unless you use a compiled verison). You can install rust here:

https://www.rust-lang.org/tools/install

after installing, you can check to see if it installed correctly by running:

rustc --version

If this does not work then try this before trying the version command again on a new terminal window:

source $HOME/.cargo/env

To run the application, in the terminal you need to provide two arguments.

1. The search string
2. The path to the file in which to search

cargo run -- searchstring example-filename.txt

Here is an example:

cargo run -- This test.txt > output.txt

If you want to ignore case, you can set an env variable like this:

IGNORE_CASE=1 cargo run -- this test.txt > output.txt
