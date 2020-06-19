//
// Source code recreated from a .class file by IntelliJ IDEA
// (powered by Fernflower decompiler)
//

package com.company;

import java.io.IOException;
import java.util.Scanner;

class CLI {
    CLI() {
    }

    public static void main(String[] args) throws IOException {
        Scanner scan = new Scanner(System.in);
        Parser par = new Parser();
        Terminal terminal = new Terminal();

        while(true) {
            String s = scan.nextLine();

            try {
                if (par.parse(s)) {
                    if (par.command.compareTo("cd") == 0) {
                        terminal.cd(par.arg1);
                    } else if (par.command.compareTo("mv") == 0) {
                        terminal.mv(par.arg1, par.arg2);
                    } else if (par.command.compareTo("mkdir") == 0) {
                        terminal.mkdir(par.arg1);
                    } else if (par.command.compareTo("rmdir") == 0) {
                        terminal.rmdir(par.arg1);
                    } else if (par.command.compareTo("rm") == 0) {
                        terminal.rm(par.arg1);
                    } else if (par.command.compareTo("ls") == 0) {
                        terminal.ls();
                    } else if (par.command.compareTo("cat") == 0) {
                        terminal.cat(par.arg1);
                    } else if (par.command.compareTo("cp") == 0) {
                        terminal.cp(par.arg1, par.arg2);
                    } else if (par.command.compareTo("echo") == 0) {
                        terminal.echo(par.arg1);
                    } else if (par.command.compareTo("clear") == 0) {
                        terminal.clear();
                    } else {
                        terminal.pwd();
                    }
                }
            } catch (IOException var6) {
                System.out.println(var6.getMessage());
            }
        }
    }
}
