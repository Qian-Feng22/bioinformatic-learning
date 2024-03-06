# bioinformatic-learning

For bioinformatics learning 2024 spring

**Learing plan for bioinformatic course**
- Follow the whole course and improve the ability of using Linux, R and Python. 
- Try to discuss with others, learn from peers and find more learning source
- Polish the ability to use computer
- Practise makes perfect, spend more time practicing coding

**Note for the first class**

 Five top rank questions released in _Science_, among which "Why humans have so few genes?" is related to what we do today.
- RNA types, including coding and noncoding RNA. The noncoding RNA maybe the key to answer to this question.
- Linux bash, good at deal with large quantity of files.
- R, good at plot and analyze datas.
- Python, good at both sides but not an expert in both fields.

 The difference between **alogrithm** and **model** is as follows
- **Alogrithm**, is a standard step by step procedure and rules to solve specific problems or tasks.
- **Model**, is a representation or approximation of the underlying structure of the data and the result of applying an algorithm to a set of data

*update on 3.3.2024*

```bash
test@QianFeng_docker:~/share$ wc -l test_command.gtf
test@QianFeng_docker:~/share$ wc -c test_command.gtf

test@QianFeng_docker:~/share$ grep 'chr_' test_command.gtf | grep 'gene_id "YDL248W"'

test@QianFeng_docker:~/share$ sed 's/chr_/chromosome_/g' test_command.gtf | awk '{print $1, $3, $4, $5}'

test@QianFeng_docker:~/share$ man awk
test@QianFeng_docker:~/share$ awk '{temp=$2; $2=$3; $3=temp; print $0}' test_command.gtf | sort -k4,4n -k5,5n > result.gtf

test@QianFeng_docker:~/share$ ls -l test_command.gtf
-rwx-wx--x 1 test test 636 Mar  6 08:03 test_command.gtf
test@QianFeng_docker:~/share$ chmod u=rwx,g=rwx,o=r test_command.gtf
test@QianFeng_docker:~/share$ ls -l test_command.gtf
-rwxrwxr-- 1 test test 636 Mar  6 08:03 test_command.gtf
```
