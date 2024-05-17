### Висновки

#### Жадібний алгоритм

Жадібний алгоритм (Greedy Algorithm) працює за принципом вибору найбільшого доступного номіналу монети на кожному кроці. Для нашого набору монет `[50, 25, 10, 5, 2, 1]`, цей підхід дуже ефективний, оскільки завжди обирає оптимальну комбінацію монет, використовуючи мінімальну кількість монет. Алгоритм має часову складність \(O(n)\), де \(n\) — кількість різних номіналів монет. 

Жадібний алгоритм працює добре для цього конкретного набору монет, але не завжди гарантує оптимальне рішення для всіх можливих наборів номіналів. Наприклад, якщо б ми мали набір монет `[1, 3, 4]`, для суми 6 жадібний алгоритм вибрав би монети `{4, 1, 1}`, тоді як оптимальним рішенням є `{3, 3}`.

#### Динамічне програмування

Алгоритм динамічного програмування (Dynamic Programming) використовує метод запам'ятовування результатів попередніх обчислень для побудови оптимального рішення. Цей підхід гарантує знаходження мінімальної кількості монет для будь-якої суми. Алгоритм має часову складність \(O(n \times m)\), де \(n\) — кількість різних номіналів монет, а \(m\) — сума, яку потрібно видати.

Алгоритм динамічного програмування завжди знайде оптимальне рішення, але може бути менш ефективним для великих сум через більшу складність. Проте, він універсальний і підходить для будь-яких наборів монет, забезпечуючи мінімальну кількість монет для заданої суми.

### Порівняння та висновки

1. **Час виконання**:
   - Жадібний алгоритм швидкий та ефективний для конкретного набору монет з часовою складністю \(O(n)\).
   - Алгоритм динамічного програмування має вищу часову складність \(O(n \times m)\) і може бути повільнішим для великих сум, але він гарантує оптимальне рішення.

2. **Ефективність для великих сум**:
   - Жадібний алгоритм може не знайти оптимальне рішення для деяких наборів монет, але для нашого конкретного набору він працює ефективно.
   - Алгоритм динамічного програмування завжди знайде оптимальне рішення, але може вимагати більше часу для великих сум.

### Висновок

Жадібний алгоритм є простим і швидким рішенням, яке працює добре для конкретних наборів монет, таких як [50, 25, 10, 5, 2, 1]. Однак, він не завжди гарантує оптимальне рішення для всіх можливих наборів. Алгоритм динамічного програмування, навпаки, є універсальним і завжди знайде оптимальне рішення, хоча він може бути менш ефективним з точки зору часу виконання для великих сум. Вибір між цими алгоритмами залежить від специфіки задачі та вимог до оптимальності та швидкості рішення.