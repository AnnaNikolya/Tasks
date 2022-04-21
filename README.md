# #задачаДня 
Решаем на вашем любимом языке! Решения как всегда присылаем скрытым кодом или ссылкой на гитхаб в чат с хештегом решениеДня ! Удачи:)

На собеседовании вам предлагается написать алгоритм для проверки того, может ли заданная строка s быть составлена   из двух других строк, part1 и part2.

Ограничение состоит в том, что символы в частях part1 и part2 должны быть в том же порядке, что и в s.

Интервьюер дает вам следующий пример и говорит вам выяснить остальное из заданных тестовых случаев.

Например:
'codewars' is a merge from 'cdw' and 'oears':

    s:  c o d e w a r s   = codewars
part1:  c   d   w         = cdw
part2:    o   e   a r s   = oears

Тестовые данные (ассерты библиотекой Chai):

describe("isMerge", function() {
  it('can handle som basic cases', function() {
    doTest(true, 'xcyc', 'xc', 'yc');
    doTest(true, 'xcyc', 'yc', 'xc');
    doTest(true, 'xcyc', 'xc', 'cy');
    doTest(true, 'xcyc', 'cy', 'xc');

    doTest(true, 'codewars', 'code', 'wars');
    doTest(true, 'codewars', 'cdwr', 'oeas');
    doTest(true, 'Making progress', 'Mak pross', 'inggre');
    doTest(false, 'codewars', 'code', 'code');
    doTest(false, 'More progress', 'More ess', 'pro');
  });
});
