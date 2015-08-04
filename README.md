# Picobot-Maze-etc
0 *x** -> e 1 # East has priority as it's always right side from the northern POV
0 xE** -> n 0 # if can't go east, go north
0 ne** -> x 2 # if not east or north, then take west path


1 ***x -> s 3 # south has priority from east POV
1 *x*s -> e 1 # then east
1 *e*s -> x 0 # finally north


2 x*** -> n 0 # North is east of west
2 N*x* -> w 2 # West if not able to go north
2 n*w* -> x 3 # finally south

3 **x* -> w 2 # West has priority from south POV
3 **Wx -> s 3 # 2nd priority
3 **ws -> x 1 # Last priority 
