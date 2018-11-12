# Spark Scala Word Count of Sly Fox
44564 Spark Word Count Assignment

## Me:
Jesse Alford II

## Objective:
Visualize the most frequent words used in the short story Sly Fox

## Raw Data:
Short Story, Sly Fox
Written By Beulah Murrelle
Source: http://textfiles.com/stories/13chil.txt

## Commands Used:

```
val inputFile = sc.textFile("slyFox.txt")
val tmp1 = filcountry.map(_.split(" ")).map( p=>p(1))
val fin = tmp1.flatMap(line => line.split("\n")).map(word => (word,1)).reduceByKey(_ + _);
fin.saveAsTextFile("outputDestination")
```

Citation: https://github.com/S530484/Spark_wordcount

## Results:

Discussion:
  My results show the word count of each word used in the story "Sly Fox". As expected basic connecting words like "the, and, to, etc" are the highest count words. Excluding those words you get other expected high count words like "Sly, Fox, and Rabbit".
word	count
the	74
and	57
to	39
Sly	25
he	25
a	24
of	22
Rabbit	21
his	18
Fox	18
with	17
in	17
little	15
Mrs	14
as	13
on	13
had	12
for	12
Mr	11
they	9
so	9
Papa	8
Rabbit	8
be	8
at	8
you	8
were	8
them	7
family	7
rabs	7
their	7
her	7
that	7
we	6
out	6
she	6
old	6
all	6
thought	6
have	5
our	5
my	5
quickly	5
Mama	5
will	5
Hedgehog	5
Fox	5
home	5
was	5
where	5
over	4
is	4
come	4
this	4
field	4
sack	4
never	4
it	4
The	4
not	4
mother	4
but	4
across	4
I	4
ran	4
said	4
by	4
left	4
Good	4
rabs	3
Rabbit	3
going	3
long	3
now	3
greedy	3
house	3
dinner	3
too	3
there	3
threw	3
down	3
cried	3
began	3
Hedgehog	3
toward	3
replied	3
would	3
before	3
He	3
Old	3
hounds	3
time	3
an	3
made	3
dogs	3
jumped	3
been	2
any	2
quills	2
porch	2
tree	2
eat	2
when	2
baying	2
sat	2
hole	2
found	2
After	2
log	2
has	2
us	2
after	2
covered	2
stop	2
went	2
right	2
fright	2
heard	2
grasshoppers	2
big	2
some	2
pine	2
morning	2
looked	2
just	2
quills	2
Meanwhile	2
Well	2
suddenly	2
them	2
into	2
own	2
agreed	2
came	2
one	2
eyes	2
trotted	2
sack	2
from	2
him	2
among	2
sitting	2
Why	2
grin	2
young	2
Piney	2
I	2
end	2
Mother	2
hollow	2
great	2
cozy	2
music	2
home	2
Every	2
happily	2
about	2
slight	2
brook	2
answered	2
trying	2
walking	2
Mr	2
which	2
ground	2
did	2
cried	2
Sniff	2
much	2
put	2
no	2
off	2
like	2
might	2
Fox	2
good	2
Do	2
fox	2
Oh	2
herself	2
moved	2
Sniff	2
Sniff	2
became	2
tea	1
under	1
reading	1
shot	1
do	1
leaf	1
filled	1
deep	1
very	1
hidden	1
day	1
robe	1
This	1
going	1
excited	1
leaving	1
cream	1
stayed	1
Eedgehog	1
long	1
knows	1
yard	1
prayers	1
hunters	1
Woof	1
Woods	1
Woods	1
parts	1
are	1
Lived	1
bag	1
away	1
exclaimed	1
dinner	1
morning	1
door	1
Call	1
soft	1
meadows	1
Sly	1
readily	1
heavily	1
silvery	1
voice	1
red-coated	1
us	1
tender	1
Into	1
planned	1
delighted	1
road	1
trapped	1
lived	1
air	1
birds	1
again	1
beside	1
earth	1
sharp	1
closer	1
as	1
busily	1
us	1
evening	1
enemy	1
am	1
even	1
getting	1
dig	1
stick	1
do	1
shall	1
same	1
new	1
lost	1
We	1
Squirrels	1
My	1
breath	1
again	1
chocolate	1
heart	1
quiet	1
chase	1
porch	1
Why	1
frown	1
lovingly	1
fire	1
don't	1
bring	1
bother	1
death	1
woods	1
places	1
As	1
I	1
How	1
morning	1
Rabbit	1
yesterday	1
But	1
mint	1
three	1
Woof	1
chat	1
together	1
prayers	1
lips	1
we	1
Get	1
me	1
him	1
furiously	1
burrowed	1
walked	1
dressed	1
resist	1
near	1
hear	1
cautioned	1
She	1
straightened	1
Fox	1
frightened	1
chase	1
rubber	1
Is	1
upon	1
until	1
rain	1
hair	1
Looks	1
only	1
wind	1
disappointed	1
here	1
mice	1
trembling	1
piled	1
Suddenly	1
Woof	1
go	1
slippers	1
poor	1
unknown	1
asked	1
merrily	1
What	1
crystal	1
sack	1
Late	1
concern	1
cunning	1
talking	1
calling	1
road	1
still	1
bushes	1
night	1
tomorrow	1
closer	1
can	1
real	1
chuckling	1
needles	1
Father	1
feet	1
eyes	1
how	1
Since	1
politely	1
none	1
tired	1
life	1
again	1
dinner	1
bedroom	1
horns	1
destroy	1
sit	1
head	1
want	1
beat	1
in	1
bound	1
exclaimed	1
foolish	1
stream	1
down	1
rude	1
high	1
went	1
Go	1
knitting	1
They	1
Shading	1
horns	1
there	1
Wow	1
first	1
start	1
obedient	1
crawled	1
nuts	1
resolved	1
thumping	1
want	1
flowered	1
neighbor	1
quiet	1
whispering	1
rabs	1
rhythm	1
Throwing	1
goodies	1
well	1
eating	1
open	1
been	1
flowers	1
woodland	1
TootToot	1
day	1
himself	1
praise	1
shoulder	1
asked:	1
jumping	1
slid	1
deep	1
barking	1
wading	1
turned	1
get	1
very	1
apple	1
scratching	1
dropped	1
frightened	1
door	1
slippers	1
crickets	1
tree	1
inwardly	1
tree	1
himself	1
bulging	1
thinking	1
slowly	1
Come	1
next	1
mouth	1
softly	1
failed	1
allow	1
chirped	1
full	1
having	1
boots	1
such	1
fall	1
behaved	1
could	1
Nearer	1
told	1
through	1
Fox	1
fro	1
seen	1
look	1
place	1
chair	1
pays	1
Toot	1
mother	1
engagement	1
way	1
carpeting	1
fooled	1
called	1
Her	1
No	1
cordially	1
hunters	1
eaten	1
horses'	1
if	1
At	1
whipped	1
pull	1
nearer	1
today	1
Then	1
hill	1
digging	1
pass	1
instructed	1
Owls	1
paws	1
distance	1
ran	1
move	1
face	1
tonight	1
Up	1
clear	1
art	1
looking	1
ran	1
feast	1
But	1
sailing	1
Greediness	1
let	1
pretended	1
gone	1
pines	1
stay	1
rake	1
pines	1
rocking	1
trees	1
Nothing	1
last	1
Sorry	1
knocked	1
Won't	1
hooted	1
face	1
gave	1
living	1
up	1
Next	1
was	1
seat	1
stood	1
panic	1
Home	1
running	1
paws	1
soon	1
fragrance	1
catch	1
pulling	1
housecoat	1
or	1
apples	1
urged	1
enjoy	1
moved	1
Wishing	1
whispered	1
shaking	1
wicked	1
sang	1
suspicious	1
silly	1
digging	1
reach	1
straw	1
direction	1
making	1
alarm	1
dainty	1
cooked	1
tomorrow	1
whispered	1
Hedgehog	1
carrot	1
throughout	1
Oh	1
back	1
water	1
Wow	1
running	1
us	1
newspaper	1
A	1
grabbed	1
sight	1
socks	1
cover	1
you	1
played	1
side	1
bake	1
screaming	1
spied	1
darting	1
inquired	1
ears	1
Safe	1
your	1
It's	1
coming	1
up	1
scent	1
offered	1
her	1
chuckled	1
Ah	1
then	1
haven't	1
time	1
nice	1
hearts	1
started	1
hot	1
It	1
smacking	1
things	1
red	1
If	1
dumplings	1
wants	1
replied:	1
number	1
Take	1
grasshoppers	1
stopped	1
said	1
around	1
took	1
grasshoppers	1
huge	1
relief	1
else	1
me	1
herself	1
In	1
take	1
spectacles	1
while	1
Fox	1
dry	1
hedgehog	1
Hedgehog's	1
hustled	1
Yes	1
minnows	1
way	1
listen	1
brook	1
bothered	1
After	1
bake	1
The	1
dogs	1
loudly	1
front	1
dribbling	1
boats	1
deilicious	1
dainty	1
begun	1
greed	1
oak	1
been	1
and	1
towering	1
you	1
heaven	1
honey	1
tell	1
ears	1
fairly	1
opposite	1
home	1
thanksgiving	1

| word         | count |
|--------------|-------|
| the          | 74    |
| and          | 57    |
| to           | 39    |
| Sly          | 25    |
| he           | 25    |
| a            | 24    |
| of           | 22    |
| Rabbit       | 21    |
| his          | 18    |
| Fox          | 18    |
| with         | 17    |
| in           | 17    |
| little       | 15    |
| Mrs          | 14    |
| as           | 13    |
| on           | 13    |
| had          | 12    |
| for          | 12    |
| Mr           | 11    |
| they         | 9     |
| so           | 9     |
| Papa         | 8     |
| Rabbit       | 8     |
| be           | 8     |
| at           | 8     |
| you          | 8     |
| were         | 8     |
| them         | 7     |
| family       | 7     |
| rabs         | 7     |
| their        | 7     |
| her          | 7     |
| that         | 7     |
| we           | 6     |
| out          | 6     |
| she          | 6     |
| old          | 6     |
| all          | 6     |
| thought      | 6     |
| have         | 5     |
| our          | 5     |
| my           | 5     |
| quickly      | 5     |
| Mama         | 5     |
| will         | 5     |
| Hedgehog     | 5     |
| Fox          | 5     |
| home         | 5     |
| was          | 5     |
| where        | 5     |
| over         | 4     |
| is           | 4     |
| come         | 4     |
| this         | 4     |
| field        | 4     |
| sack         | 4     |
| never        | 4     |
| it           | 4     |
| The          | 4     |
| not          | 4     |
| mother       | 4     |
| but          | 4     |
| across       | 4     |
| I            | 4     |
| ran          | 4     |
| said         | 4     |
| by           | 4     |
| left         | 4     |
| Good         | 4     |
| rabs         | 3     |
| Rabbit       | 3     |
| going        | 3     |
| long         | 3     |
| now          | 3     |
| greedy       | 3     |
| house        | 3     |
| dinner       | 3     |
| too          | 3     |
| there        | 3     |
| threw        | 3     |
| down         | 3     |
| cried        | 3     |
| began        | 3     |
| Hedgehog     | 3     |
| toward       | 3     |
| replied      | 3     |
| would        | 3     |
| before       | 3     |
| He           | 3     |
| Old          | 3     |
| hounds       | 3     |
| time         | 3     |
| an           | 3     |
| made         | 3     |
| dogs         | 3     |
| jumped       | 3     |
| been         | 2     |
| any          | 2     |
| quills       | 2     |
| porch        | 2     |
| tree         | 2     |
| eat          | 2     |
| when         | 2     |
| baying       | 2     |
| sat          | 2     |
| hole         | 2     |
| found        | 2     |
| After        | 2     |
| log          | 2     |
| has          | 2     |
| us           | 2     |
| after        | 2     |
| covered      | 2     |
| stop         | 2     |
| went         | 2     |
| right        | 2     |
| fright       | 2     |
| heard        | 2     |
| grasshoppers | 2     |
| big          | 2     |
| some         | 2     |
| pine         | 2     |
| morning      | 2     |
| looked       | 2     |
| just         | 2     |
| quills       | 2     |
| Meanwhile    | 2     |
| Well         | 2     |
| suddenly     | 2     |
| them         | 2     |
| into         | 2     |
| own          | 2     |
| agreed       | 2     |
| came         | 2     |
| one          | 2     |
| eyes         | 2     |
| trotted      | 2     |
| sack         | 2     |
| from         | 2     |
| him          | 2     |
| among        | 2     |
| sitting      | 2     |
| Why          | 2     |
| grin         | 2     |
| young        | 2     |
| Piney        | 2     |
| I            | 2     |
| end          | 2     |
| Mother       | 2     |
| hollow       | 2     |
| great        | 2     |
| cozy         | 2     |
| music        | 2     |
| home         | 2     |
| Every        | 2     |
| happily      | 2     |
| about        | 2     |
| slight       | 2     |
| brook        | 2     |
| answered     | 2     |
| trying       | 2     |
| walking      | 2     |
| Mr           | 2     |
| which        | 2     |
| ground       | 2     |
| did          | 2     |
| cried        | 2     |
| Sniff        | 2     |
| much         | 2     |
| put          | 2     |
| no           | 2     |
| off          | 2     |
| like         | 2     |
| might        | 2     |
| Fox          | 2     |
| good         | 2     |
| Do           | 2     |
| fox          | 2     |
| Oh           | 2     |
| herself      | 2     |
| moved        | 2     |
| Sniff        | 2     |
| Sniff        | 2     |
| became       | 2     |
| tea          | 1     |
| under        | 1     |
| reading      | 1     |
| shot         | 1     |
| do           | 1     |
| leaf         | 1     |
| filled       | 1     |
| deep         | 1     |
| very         | 1     |
| hidden       | 1     |
| day          | 1     |
| robe         | 1     |
| This         | 1     |
| going        | 1     |
| excited      | 1     |
| leaving      | 1     |
| cream        | 1     |
| stayed       | 1     |
| Eedgehog     | 1     |
| long         | 1     |
| knows        | 1     |
| yard         | 1     |
| prayers      | 1     |
| hunters      | 1     |
| Woof         | 1     |
| Woods        | 1     |
| Woods        | 1     |
| parts        | 1     |
| are          | 1     |
| Lived        | 1     |
| bag          | 1     |
| away         | 1     |
| exclaimed    | 1     |
| dinner       | 1     |
| morning      | 1     |
| door         | 1     |
| Call         | 1     |
| soft         | 1     |
| meadows      | 1     |
| Sly          | 1     |
| readily      | 1     |
| heavily      | 1     |
| silvery      | 1     |
| voice        | 1     |
| red-coated   | 1     |
| us           | 1     |
| tender       | 1     |
| Into         | 1     |
| planned      | 1     |
| delighted    | 1     |
| road         | 1     |
| trapped      | 1     |
| lived        | 1     |
| air          | 1     |
| birds        | 1     |
| again        | 1     |
| beside       | 1     |
| earth        | 1     |
| sharp        | 1     |
| closer       | 1     |
| as           | 1     |
| busily       | 1     |
| us           | 1     |
| evening      | 1     |
| enemy        | 1     |
| am           | 1     |
| even         | 1     |
| getting      | 1     |
| dig          | 1     |
| stick        | 1     |
| do           | 1     |
| shall        | 1     |
| same         | 1     |
| new          | 1     |
| lost         | 1     |
| We           | 1     |
| Squirrels    | 1     |
| My           | 1     |
| breath       | 1     |
| again        | 1     |
| chocolate    | 1     |
| heart        | 1     |
| quiet        | 1     |
| chase        | 1     |
| porch        | 1     |
| Why          | 1     |
| frown        | 1     |
| lovingly     | 1     |
| fire         | 1     |
| don't        | 1     |
| bring        | 1     |
| bother       | 1     |
| death        | 1     |
| woods        | 1     |
| places       | 1     |
| As           | 1     |
| I            | 1     |
| How          | 1     |
| morning      | 1     |
| Rabbit       | 1     |
| yesterday    | 1     |
| But          | 1     |
| mint         | 1     |
| three        | 1     |
| Woof         | 1     |
| chat         | 1     |
| together     | 1     |
| prayers      | 1     |
| lips         | 1     |
| we           | 1     |
| Get          | 1     |
| me           | 1     |
| him          | 1     |
| furiously    | 1     |
| burrowed     | 1     |
| walked       | 1     |
| dressed      | 1     |
| resist       | 1     |
| near         | 1     |
| hear         | 1     |
| cautioned    | 1     |
| She          | 1     |
| straightened | 1     |
| Fox          | 1     |
| frightened   | 1     |
| chase        | 1     |
| rubber       | 1     |
| Is           | 1     |
| upon         | 1     |
| until        | 1     |
| rain         | 1     |
| hair         | 1     |
| Looks        | 1     |
| only         | 1     |
| wind         | 1     |
| disappointed | 1     |
| here         | 1     |
| mice         | 1     |
| trembling    | 1     |
| piled        | 1     |
| Suddenly     | 1     |
| Woof         | 1     |
| go           | 1     |
| slippers     | 1     |
| poor         | 1     |
| unknown      | 1     |
| asked        | 1     |
| merrily      | 1     |
| What         | 1     |
| crystal      | 1     |
| sack         | 1     |
| Late         | 1     |
| concern      | 1     |
| cunning      | 1     |
| talking      | 1     |
| calling      | 1     |
| road         | 1     |
| still        | 1     |
| bushes       | 1     |
| night        | 1     |
| tomorrow     | 1     |
| closer       | 1     |
| can          | 1     |
| real         | 1     |
| chuckling    | 1     |
| needles      | 1     |
| Father       | 1     |
| feet         | 1     |
| eyes         | 1     |
| how          | 1     |
| Since        | 1     |
| politely     | 1     |
| none         | 1     |
| tired        | 1     |
| life         | 1     |
| again        | 1     |
| dinner       | 1     |
| bedroom      | 1     |
| horns        | 1     |
| destroy      | 1     |
| sit          | 1     |
| head         | 1     |
| want         | 1     |
| beat         | 1     |
| in           | 1     |
| bound        | 1     |
| exclaimed    | 1     |
| foolish      | 1     |
| stream       | 1     |
| down         | 1     |
| rude         | 1     |
| high         | 1     |
| went         | 1     |
| Go           | 1     |
| knitting     | 1     |
| They         | 1     |
| Shading      | 1     |
| horns        | 1     |
| there        | 1     |
| Wow          | 1     |
| first        | 1     |
| start        | 1     |
| obedient     | 1     |
| crawled      | 1     |
| nuts         | 1     |
| resolved     | 1     |
| thumping     | 1     |
| want         | 1     |
| flowered     | 1     |
| neighbor     | 1     |
| quiet        | 1     |
| whispering   | 1     |
| rabs         | 1     |
| rhythm       | 1     |
| Throwing     | 1     |
| goodies      | 1     |
| well         | 1     |
| eating       | 1     |
| open         | 1     |
| been         | 1     |
| flowers      | 1     |
| woodland     | 1     |
| TootToot     | 1     |
| day          | 1     |
| himself      | 1     |
| praise       | 1     |
| shoulder     | 1     |
| asked:       | 1     |
| jumping      | 1     |
| slid         | 1     |
| deep         | 1     |
| barking      | 1     |
| wading       | 1     |
| turned       | 1     |
| get          | 1     |
| very         | 1     |
| apple        | 1     |
| scratching   | 1     |
| dropped      | 1     |
| frightened   | 1     |
| door         | 1     |
| slippers     | 1     |
| crickets     | 1     |
| tree         | 1     |
| inwardly     | 1     |
| tree         | 1     |
| himself      | 1     |
| bulging      | 1     |
| thinking     | 1     |
| slowly       | 1     |
| Come         | 1     |
| next         | 1     |
| mouth        | 1     |
| softly       | 1     |
| failed       | 1     |
| allow        | 1     |
| chirped      | 1     |
| full         | 1     |
| having       | 1     |
| boots        | 1     |
| such         | 1     |
| fall         | 1     |
| behaved      | 1     |
| could        | 1     |
| Nearer       | 1     |
| told         | 1     |
| through      | 1     |
| Fox          | 1     |
| fro          | 1     |
| seen         | 1     |
| look         | 1     |
| place        | 1     |
| chair        | 1     |
| pays         | 1     |
| Toot         | 1     |
| mother       | 1     |
| engagement   | 1     |
| way          | 1     |
| carpeting    | 1     |
| fooled       | 1     |
| called       | 1     |
| Her          | 1     |
| No           | 1     |
| cordially    | 1     |
| hunters      | 1     |
| eaten        | 1     |
| horses'      | 1     |
| if           | 1     |
| At           | 1     |
| whipped      | 1     |
| pull         | 1     |
| nearer       | 1     |
| today        | 1     |
| Then         | 1     |
| hill         | 1     |
| digging      | 1     |
| pass         | 1     |
| instructed   | 1     |
| Owls         | 1     |
| paws         | 1     |
| distance     | 1     |
| ran          | 1     |
| move         | 1     |
| face         | 1     |
| tonight      | 1     |
| Up           | 1     |
| clear        | 1     |
| art          | 1     |
| looking      | 1     |
| ran          | 1     |
| feast        | 1     |
| But          | 1     |
| sailing      | 1     |
| Greediness   | 1     |
| let          | 1     |
| pretended    | 1     |
| gone         | 1     |
| pines        | 1     |
| stay         | 1     |
| rake         | 1     |
| pines        | 1     |
| rocking      | 1     |
| trees        | 1     |
| Nothing      | 1     |
| last         | 1     |
| Sorry        | 1     |
| knocked      | 1     |
| Won't        | 1     |
| hooted       | 1     |
| face         | 1     |
| gave         | 1     |
| living       | 1     |
| up           | 1     |
| Next         | 1     |
| was          | 1     |
| seat         | 1     |
| stood        | 1     |
| panic        | 1     |
| Home         | 1     |
| running      | 1     |
| paws         | 1     |
| soon         | 1     |
| fragrance    | 1     |
| catch        | 1     |
| pulling      | 1     |
| housecoat    | 1     |
| or           | 1     |
| apples       | 1     |
| urged        | 1     |
| enjoy        | 1     |
| moved        | 1     |
| Wishing      | 1     |
| whispered    | 1     |
| shaking      | 1     |
| wicked       | 1     |
| sang         | 1     |
| suspicious   | 1     |
| silly        | 1     |
| digging      | 1     |
| reach        | 1     |
| straw        | 1     |
| direction    | 1     |
| making       | 1     |
| alarm        | 1     |
| dainty       | 1     |
| cooked       | 1     |
| tomorrow     | 1     |
| whispered    | 1     |
| Hedgehog     | 1     |
| carrot       | 1     |
| throughout   | 1     |
| Oh           | 1     |
| back         | 1     |
| water        | 1     |
| Wow          | 1     |
| running      | 1     |
| us           | 1     |
| newspaper    | 1     |
| A            | 1     |
| grabbed      | 1     |
| sight        | 1     |
| socks        | 1     |
| cover        | 1     |
| you          | 1     |
| played       | 1     |
| side         | 1     |
| bake         | 1     |
| screaming    | 1     |
| spied        | 1     |
| darting      | 1     |
| inquired     | 1     |
| ears         | 1     |
| Safe         | 1     |
| your         | 1     |
| It's         | 1     |
| coming       | 1     |
| up           | 1     |
| scent        | 1     |
| offered      | 1     |
| her          | 1     |
| chuckled     | 1     |
| Ah           | 1     |
| then         | 1     |
| haven't      | 1     |
| time         | 1     |
| nice         | 1     |
| hearts       | 1     |
| started      | 1     |
| hot          | 1     |
| It           | 1     |
| smacking     | 1     |
| things       | 1     |
| red          | 1     |
| If           | 1     |
| dumplings    | 1     |
| wants        | 1     |
| replied:     | 1     |
| number       | 1     |
| Take         | 1     |
| grasshoppers | 1     |
| stopped      | 1     |
| said         | 1     |
| around       | 1     |
| took         | 1     |
| grasshoppers | 1     |
| huge         | 1     |
| relief       | 1     |
| else         | 1     |
| me           | 1     |
| herself      | 1     |
| In           | 1     |
| take         | 1     |
| spectacles   | 1     |
| while        | 1     |
| Fox          | 1     |
| dry          | 1     |
| hedgehog     | 1     |
| Hedgehog's   | 1     |
| hustled      | 1     |
| Yes          | 1     |
| minnows      | 1     |
| way          | 1     |
| listen       | 1     |
| brook        | 1     |
| bothered     | 1     |
| After        | 1     |
| bake         | 1     |
| The          | 1     |
| dogs         | 1     |
| loudly       | 1     |
| front        | 1     |
| dribbling    | 1     |
| boats        | 1     |
| deilicious   | 1     |
| dainty       | 1     |
| begun        | 1     |
| greed        | 1     |
| oak          | 1     |
| been         | 1     |
| and          | 1     |
| towering     | 1     |
| you          | 1     |
| heaven       | 1     |
| honey        | 1     |
| tell         | 1     |
| ears         | 1     |
| fairly       | 1     |
| opposite     | 1     |
| home         | 1     |
| thanksgiving | 1     |

![Results](https://i.imgur.com/DSTXIYS.png)
