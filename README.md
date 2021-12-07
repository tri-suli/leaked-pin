# Leaked PIN

Username dan Hashed PIN milik PT SerbaTerbuka bocor di sebuah forum Hacker. "Tenang saja, PINnya sudah diamankan dengan hash function yang kuat", kata juru bicara di PT SerbaTerbuka tersebut.

Bob merasa ada yang janggal dari pernyataan tersebut. Setelah digali lebih dalam, Bob mendapati informasi berikut:

Hash function h yang digunakan adalah: h(k) = k * (k+3) mod 1000003, di mana k adalah key yang ingin dihash

PIN adalah angka (0-9) dengan panjang tepat N digit

Sebagian Hashed PIN ternyata tidak valid, kemungkinan hackernya sengaja merusak sebagian nilainya

Dengan data tersebut, bantu Bob mendapati PIN semua orang

Input
Baris pertama adalah T jumlah test cases. 1 <= T <= 100
T baris berikutnya adalah N dan Hashed PIN, dipisahkan oleh spasi
0 <= Hashed PIN < 1000003
Test Set 1
1 <= N <= 6
Test Set 2
7 <= N <= 8
Output
Untuk masing-masing test case, print 1 baris dengan format Case #i: PINS, di mana i adalah nomor test casenya (dimulai dari 1) dan PINS adalah kemungkinan PIN
Jika ada lebih dari satu kemungkinan PIN, tampilkan semuanya dengan dipisahkan spasi, urutkan dari yang paling kecil
Jika Hashed PIN tidak valid, tampilkan Invalid
Sample Input 1
5
1 28
2 18
4 10300
6 10300
1 5
Sample Output 1
Case #1: 4
Case #2: 03
Case #3: 0100
Case #4: 000100 999900
Case #5: Invalid
Explanation
Untuk Case #1, h(4) = 4 * (4 + 3) mod 1000003 = 28
Untuk Case #4, h(000100) = 10300 dan h(999900) = 10300
Sample Input 2
2
7 598786
8 63003
Sample Output 2
Case #1: Invalid
Case #2: 00227527 00772473 01227530 01772476 02227533 02772479 03227536 03772482 04227539 04772485 05227542 05772488 06227545 06772491 07227548 07772494 08227551 08772497 09227554 09772500 10227557 10772503 11227560 11772506 12227563 12772509 13227566 13772512 14227569 14772515 15227572 15772518 16227575 16772521 17227578 17772524 18227581 18772527 19227584 19772530 20227587 20772533 21227590 21772536 22227593 22772539 23227596 23772542 24227599 24772545 25227602 25772548 26227605 26772551 27227608 27772554 28227611 28772557 29227614 29772560 30227617 30772563 31227620 31772566 32227623 32772569 33227626 33772572 34227629 34772575 35227632 35772578 36227635 36772581 37227638 37772584 38227641 38772587 39227644 39772590 40227647 40772593 41227650 41772596 42227653 42772599 43227656 43772602 44227659 44772605 45227662 45772608 46227665 46772611 47227668 47772614 48227671 48772617 49227674 49772620 50227677 50772623 51227680 51772626 52227683 52772629 53227686 53772632 54227689 54772635 55227692 55772638 56227695 56772641 57227698 57772644 58227701 58772647 59227704 59772650 60227707 60772653 61227710 61772656 62227713 62772659 63227716 63772662 64227719 64772665 65227722 65772668 66227725 66772671 67227728 67772674 68227731 68772677 69227734 69772680 70227737 70772683 71227740 71772686 72227743 72772689 73227746 73772692 74227749 74772695 75227752 75772698 76227755 76772701 77227758 77772704 78227761 78772707 79227764 79772710 80227767 80772713 81227770 81772716 82227773 82772719 83227776 83772722 84227779 84772725 85227782 85772728 86227785 86772731 87227788 87772734 88227791 88772737 89227794 89772740 90227797 90772743 91227800 91772746 92227803 92772749 93227806 93772752 94227809 94772755 95227812 95772758 96227815 96772761 97227818 97772764 98227821 98772767 99227824 99772770
Answer Submission Instructions
There is small case and big case score, each has its max score like shown below, your task is to get the highest possible score.
Once you run your code, your source code, small case & big case output will be automatically saved as the answer.
You may run your code as many time as you want (as long as there's still time) until you get the highest possible score.
On some programming languages, we already provide you the template that read the input data, just click Insert Template from top left menu.
The total coding score that we will assess is the sum up of all small and big case scores across all coding tests.
Please make sure the content formatting (symbols, capitalization, space, line break, etc.) of the output result from your code
must match exactly the same like in the sample output shown on the question because it will affect your scoring if you miss even a single space.
Because the data on some small/big case input is huge, so the time to execute your code can be very long. We recommend you to run
the sample case first to make sure your code is right. Note that you will not get any score from sample case, it's just a playground.
You can also edit sample input data from the editor, in case you need to debug/test your code.
