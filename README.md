# upper-and-lower-case

https://www.hackerrank.com/challenges/one-month-preparation-kit-caesar-cipher-1/problem?isFullScreen=true&h_l=interview&playlist_slugs%5B%5D=preparation-kits&playlist_slugs%5B%5D=one-month-preparation-kit&playlist_slugs%5B%5D=one-month-week-two

有大有小的字母换算：

        【笨方法】 可以建立一个大写集 + 一个小写集： 
            alphabet = 'abcdefghijklmnopqrstuvwxyz'
            alphabet_Upper = alphabet.upper()
            ans=''
            for i in range(k):
                alphabet += alphabet[i]
                alphabet_Upper += alphabet_Upper[i]

            for c in s:
                if c in alphabet:
                    index = alphabet.index(c) +k
                    ans+= alphabet[index]
                elif c in alphabet_Upper:
                    index = alphabet_Upper.index(c) + k
                    ans += alphabet_Upper[index]
                else:
                    ans += c

用ascii:
http://sticksandstones.kstrom.com/appen.html

          a-z: 97-122
          symbols_low = string.ascii_lowercase
          A-Z: 65-90
          symbols_up = string.ascii_uppercase


用ord


# 循环怎么看？

笨方法：
尾巴上加s[i]


