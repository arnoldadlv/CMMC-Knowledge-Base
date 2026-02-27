---
source: Summit 7
type: youtube-transcript
url: https://www.youtube.com/watch?v=F1qPWHx5XMM
date: June 09, 2025
tags:
  - cmmc
  - dib
  - summit7
---

# CMMC Enclaves by Industry

**Source:** [Summit 7 - YouTube](https://www.youtube.com/watch?v=F1qPWHx5XMM)
**Date:** June 09, 2025

---

## Transcript

[Music]
Hello
everybody. Welcome to a very riveting
conversation about CMMC enclaves by
industry. So at Summit 7, we have a few
different major verticals that we play
in construction, manufacturing, and
regulated research. Now that's not all
the industries, but those are the three
largest kind of pieces of our client
base. And so I get the privilege of
working with very large enterprises in
all of those spaces and very small micro
businesses in those places as well. And
so the questions get brought up, can I
do an enclave? Should I do an enclave?
Will it meet my requirements for
manufacturing, for research, for
building, right, construction, AEC work?
And the short answer is maybe. And we're
going to figure out if it's going to fit
your needs today as we go through this.
I'm very much an interactive guy. So, if
you have a question, you don't have to
wait till the end. You can just throw a
little hand up and if we're running
short on time, I might just ignore you
and then we'll get to it at the end. And
it also has to be a good question. I
don't have the red phone out here,
sadly. So, this is me uh in
2007, believe it or not. So, I'm a
recovering IT guy of 17 years. I'm a
current sales guy at Summit 7, co-host
of the lovely CUI Hotline. worked for
MSPs and Army Material Command for quite
a few years. Um, and then when I was 10,
I was a fire safety clown for the
American Red Cross. Uh, points for
anyone that can guess my name. I will
give you a CS2 t-shirt, merch, something
like that. Any
guesses. Dan the Man, that's that. I
should have been that. My mom named me
sadly, so if that gives you any
indication how great it is. Carrot top,
another good one. It was pinwheel. And I
do not have a picture of that because it
would give you nightmares if I showed
you what that actually looked like.
So let's get into all of the wonderful
points of the
powerpoints. What is an enclave? Should
you do one? Data flow and you
manufacturing enclaves, what they call
AEC, architectural engineering and
construction enclaves, regulated
research, how do I pick an enclave
vendor? Because that's a good good good
question to ask. and just general Q&A
throughout. So, first off, what is an
enclave? So, this is from the CMMC L2
scoping guidance. This pulled right out
of it. Satisfaction of CMMC security
requirements may be accomplished by
people, processes, or technologies which
apply to the entire organization seeking
assessment enterprise. This does not
mean all the assets across the entire
OSC enterprise are automatically part of
your CMMC assessment scope. All it's
saying is you don't got to put
everything inside of the box for CUI.
You get to be selective around what
people, places, technology you put in
the box, specifically the things are
going to process, store, and transmit
CUI. So you don't have to put everything
in there. We get to pick the things that
we want in there. And that's where we
start talking about data flow and things
like that.
So the first question which we're going
to answer throughout this particular
presentation is do you know where all
your CUI is? So if we think of an
enclave as a box that you're going to
put everything in. We have to know where
all the little CUI files are pieces of
paper data engineering files research.
We have to know what CUI to be able to
put it in the enclave. If you do not
know where this is, you probably
shouldn't do an
enclave, right? And I'm not saying it's
a foolproof. You might do an enclave to
start while you figure out how much
larger it needs to be long term, but as
a final solution in in your process,
it's probably not the end. It's probably
just the beginning as like a stop gap,
right? Next up, do more than 15% of your
users need access to CUI to perform the
work? This is a very common universal
kind of question that we ask because
what we have found and I think you
probably all have found out users take
the path of least resistance. If you
give them a company computer and you
give them a VDI for an enclave, uh the
more people you add to that VDI portion
of it, the more and more chances are
that people are going to try and find a
workaround, right? They're now going to,
you know, I'm just going to do it real
quick. I'm just going to send a quick
email through my commercial. Nobody will
be the wiser. I'll be okay. Right? And
you multiply that times, you know, 50,
100, 150, a thousand people, uh, you
start having a little bit of problems
with some, you know, spillage, you could
say. Um, so anyway, so that's another
good point. We have found that after
15%, the overhead to support both
environments as well as the increased
risk for spillage type activities of CUI
or export control in non-compliance
spaces goes up significantly.
Can your data flow support an enclave?
So again, an enclave in a traditional
sense, at least the way that we deploy
it, is primarily virtual desktop driven,
but doesn't have to stop there. Could be
physical devices, OT equipment, research
equipment, you name it. Right? So
question, if you get, you know, a
solicitation today, if your BD team's
working on something and they're writing
a proposal and that proposal has past
performance, that's considered CUI and
that goes over to contracts and then
contracts reviews it. When you start
going through all of that all the way
through to the deliverable stage, can an
enclave, can this separate environment
actually support the CUI data flow? It's
also fun question. And this I've heard
it three times at this conference so far
in the six hours that we've been
together. It cannot answer these
questions alone. Do not at me about
this. If you're in IT CMMC, I'm going to
validate you for a second. Is not solely
your problem. It is an executive problem
that needs to be solved by multiple
different parties because it is
traditionally supporting the
infrastructure where CUI may or may not
live. They don't exactly know if that
data is CUI or not. They need to be
informed of that. Everybody tracking so
far feeling good. All right. Riveting
stuff. I know. Data flow and you these
are a bunch of icons I got from the
PowerPoint template that we have
representing all sorts of things that
CUI can sit on. CNC machines, printers,
USBs, laptops, mobile devices, servers,
thirdparty clouds, email across the
board, right? So, you're looking at
these things and you're like, "Yes, my
business has some of these things or all
of these things." That's fantastic. The
next question is, does the CUI sit on
these things? Right? And if so, can we
remove the CUI from these and stick them
in a second environment which would be
considered the
enclave? There's a little bit of a cheat
sheet that we made and we actually
implement this on the other side as part
of our project for Xfiltration.
But if you're technical in nature or you
have access to a technical team, one of
the things we highly recommend is, and
these are just some examples, you can
send me a message on LinkedIn if you
want the full list, is go into your M365
commercial tenant, go into your
network's interest uh in instance, if
you have something for on-prim file
scanning, and just run searches for the
CUI banner markings, DoD clauses, DoD
distribution statements, and you'll
quickly find out. I think I might have
more CUI than I think I thought I had.
Um, the interesting part about this and
I I love story time because I get to
talk to a lot of fun companies. I was
talking with a large construction
company and the CIO was like, "Yeah, we
just, you know, we're going to do like a
20 person enclave." I said, "That's
fantastic." I said, "How did you get to
that number? How did 20 people appear on
your desk? These are our CUI people."
and they're like, "That's just kind of
who we think would be in scope." I said,
'You know, there's there's no no harm,
no foul in thinking that to start. I was
like, but let's do a little bit of
research. I was like, before you kind of
just sign up to build an enclave, let's
try and do a little bit more scoping.
So, they ran this and there's about a
page and a half more that you can't see
here on the screen of keywords. And they
came back to me a week ago and said,
"Daniel, we just ran ran the DoD
distribution statement part B through F
here and we got
570 files back with just
that. It feels like maybe more than 20
people probably are having access to
those 570 files, right?" And that was
just DoD distribution statements and
that was only what Microsoft could read.
OCR through PDFs, email, certain select
attachments, you know, Doc, Excel, so
forth and so on. This was not
engineering files. It wasn't scanning
AutoCAD files. It wasn't Solid Works
files, Revit files. This was just base
communication, I would say, with
traditional office-based attachments.
And so before you kind of get into the
thought of an enclave is going to be my
forever home or hey should I even do an
enclave to start doing a search like
this will do a ton it'll pay dividends
in the long term because when you go to
an executive and you knock on their door
and you say I think I saw this CMMC
thing we're going to build an enclave
right we're going to stick 20 people in
it and then you have to go back six
months later because you found out
there's way more CUI and way more people
than you thought there were the second
ask is always a little bit harder. So,
let's do one big ask uh with as much
information that we can possibly get at
our fingertips at the time and then
start framing out the size and scale of
what this enclave actually looks
like.
Okay, so Daniel, I've done the research.
I figured it out. I've got 50 users that
are going to fit in this magical little
enclave box you're talking about. Okay,
that's fantastic. We figured it out. So
depending on the industry, there's
different problems that you're going to
have over have to overcome that other
industries are not going to have to
overcome. And you could be a blend. You
might have some issues that regulated
research have in your manufacturing
space. So when we get through this,
don't tune out after your industry
because you might actually pick up
something that you need as part of yours
because you might have a very unique
case as part of
this manufacturing. This is just some
highle bullets of all the fun
conversations that we have. Needs to be
able to receive CUI in a compliant
manner. This is kind of a catch-all for
everybody. We got to figure out a way to
ingest it. And one of the hardest things
if you're running an enclave today is
training your outside people to send it
to the correct place. I tell people all
the time just like those keywords that
you see that's really good like you know
search and potentially destroy kind of
criteria, right? You can do content
searches in
M365, set up the same type of detection
patterns or sensitivity labels on
transport rules coming for data coming
into your environment because then you
can basically create a custom
non-deliverable and say, "Hey, this
appears to contain CUI. Please send it
to the correct place." And again, your
goal is to try and keep and show proof
that you're keeping those systems out of
scope of your enclave, right? Needs to
be able to leverage specific
applications to perform the work.
AutoCAD, Solid Works, etc. Right?
Engineering type tool
sets needs to be able to print drawings
for assemblies. I was on site at a
manufacturer. They they build harnesses.
They do like 90% defense stuff in the
lovely city of Huntsville, Alabama,
which I am from. Roll Todd. And um
because of that, they were like,
"Listen, we need like seven computers
that do the CUI stuff and we print it
out and then we take it into the shop
floor where there's 50 people across a
dozen desks assembling all of these
harnesses." I was like, "Okay, that's
fantastic." They're like, "So, we have
to have a printer in scope. There's just
no way around it because we're not going
to give everybody a computer. They don't
need a computer. They just need the
document in order to assemble the thing.
Okay, that's sounds sounds great. And it
needs to be able to move data into the
shop floor or OT operational technology
environment. Now, DoD gets a lot of flak
about CMMC these days, but they did
manufacturing a solid research also
falls into this category of specialized
assets. Who has played around with the
word or the asset classification of
specialized assets? Has anyone been
playing with this? All right, we got
some asset scopes in here. All right, so
when you're going through your Enclave,
you're going to run into four major
asset types. Your CUI asset, your
security protection asset, your
contractor risk manage asset, which if
you're using that, that's kind of a
trap, so be careful. Use with caution,
and your specialized assets.
Specialized assets are fun because they
can process, store, transmit CUI, but
don't have to have all the CMMC controls
on it. You're like, Daniel, that makes
no sense. I know. I know. Well, if
you're in manufacturing, you realize
that you have systems that are
supporting your CNC machines that are
still running Windows XP, Windows 2000,
MS DOSs. My favorite conversation with
somebody a few years ago because we were
talking about building out an
environment. He's like, "Daniel, I have
to go to eBay to buy scuzzy drives to
keep this system alive." And they did
laser cutting of like diamonds and chips
and cards and just really fascinating
stuff. But they're like, I have to go to
eBay and set like a little notification
whenever a scuzzy drive comes up for
sale and just have it auto buy, you
know, at $50 or less, just buy that
thing and ship it to our warehouse,
right?
So the DoD introduced this asset type
called specialized assets. Not saying
you don't have to apply any security to
them, but you have to do some sort of
riskbased security policies, procedures,
or practices and show how you're
protecting them. It does not have to be
aligned to of the 110 practices or
controls of CMMC. That might be an easy
place to start. Um, but it's definitely
worth investigating. This is also again
ties into research for systems or
equipment that just can't meet that
requirement that do perform a function
like government property, IoT, OT,
restricted infosystems, test equipment.
This is all on the CMMCL2 scoping
guidance on the DoD CIO website as well.
Um, if you want a link, just just let me
know if you don't know where that is.
So, let's get into an enclave. You're
going to see this picture morphed quite
a few times here.
So the traditional enclave that we go
through and deploy is virtual desktop
based. Typically we use Azure virtual
desktop with GPUs behind it for
engineering type applications. Right?
NVIDIA cards are are all over the place
in Azure Gov. Uh we don't have the H200
cards yet. So if you're, you know, big
high performance compute, we're getting
those. We have the H100s currently. But
anyways, we spin up a Windows 11 virtual
desktop. We slap on the applications and
we give the creds to the user and say
log in and do your job. Well, I just
made it sound very simple. There's quite
a bit of complexity to that. So, here's
a couple things to consider before I get
to the other
considerations. Virtual desktops are
great if your latency is below 70
milliseconds. How many of you run a
speed test at home before? Pretty
common, right? Hey, am I getting
everything I'm paying for? Is this
gigabit really gigabit? Right? Well, if
you're ever curious if VDI is going to
be a good solution or good
fit, talk to the person that is in the
most backwoods place you can that's
going to be accessing this and have them
run a speed test because they are going
to have a terrible experience if you
start clipping over 70
milliseconds. Um, so that's really kind
of good to know because it's not
necessarily the back-end virtual
infrastructure that's the problem. It's
the connection to the environment,
right? the latency piece of it. So, a
few other considerations when we're
talking manufacturing. If you bring on
premise into scope, meaning what we
would refer to as a hybrid enclave, uh
physical protection and security will
apply to your environment, right? So,
there's two kind of forms of an enclave.
The top cloud piece that's just running
solely in the cloud, you get to inherit
a lot of physical protections or pretty
much all physical protections from
Microsoft's SSP. Um but if you want you
connect that back on prim typically
through a sight toightVPN connection uh
now your physical site is in scope right
now how much in scope is the fun
question right is it a secure room is it
a whole facility right what does that
look like so I'll give you a few
examples I've recently worked with some
very large international machine shops
um that do manufacturing of all sorts of
incredible gizmos and 3D printing metal
and crazy stuff like that and they had
to make the decision that CUI is so
prevalent, we're going to have to make a
business decision to consolidate to
single physical sites here in the US. So
they had to look across their 50 or so
physical sites across the world,
identify the type of defense work being
done, if there was any, and then they've
made the slow progression over multiple
years to move the actual manufacturing
of that into one or two physical sites
here state side, right? So when we're
building an enclave, it could be a room,
it could be a site. One of the hard
things for manufacturing
is those actual tools, the OT
manufacturing environment is very
expensive, right? And to physically
consolidate some of those tool sets
might take you some time. So just make
sure you're thinking about the logistics
of things like that. What sites make
this particular part? Can we
consolidate? Does that does that
physical site need to be in scope now?
Right? what happens if then they're in
Malaysia or Taiwan or, you know, we've
even had conversations about what if
they're in China? A little bit of a
problem, right? Um, and so anyways,
that's one other kind of consideration
to think of as you go through
this. Physical workstations might make
more sense than virtual
desktops. That's just a harsh reality,
right? People want an enclave to
mitigate risk and to make something
compliant very fast. the calls I'm
getting now, people jump on the call and
say, ' Daniel, I've got to be CMMC
compliant. Build me an Enclave tomorrow.
I said, ' Okay, interesting. Well, well,
I talked to you five years ago and you
weren't that interested then. You know
what changed? You know, it's like, oh,
that yeah, you're being required, you
know, more so to do it now, even though
you were kind of required back then, but
anyways. And so, it takes a little bit
of time. It takes a little bit of time
to adjust your data flow to figure out
the assets that are in scope, the sites
in scope and if you need physical
devices as part of that equation or not
and not just virtual. So sales and BD
might be great on VDIs. They might be
able to support something like that. Um
but maybe your manufacturing
environment, you know, for the
engineering applications, maybe they
can't support virtual environments.
Maybe they can, right? One additional
kind of really cool thing that's pretty
new is we just launched our partnership
with a uh actually a partner here called
Hyporei. So before virtual desktops, it
was a remote desktop shortcut on your
desktop and you had to have like a
laptop to do it. Well, now Hyporei is
super cool. You have an app on your
mobile phone and you can connect to an
Android instance that's has all of the
Microsoft apps running in the GovCloud.
So now your company doesn't have to have
two physical devices, one for the
enclave and one for the corporate
environment. So now you can do VDI
through Android interfaces. It works on
iOS and Android for all your mobile
applications so your salespeople don't,
you know, throw over a table. Um, and
then you can use a Windows 11 virtual
desktop on your Windows or Mac to
connect into that, right? So it's pretty
cool. Uh, however, one fun thing and I
don't know why I put the word however
here. Print jobs are sent in plain text.
So, one of the battles that we have
fought forever, and this is me
personally going back to that 17 years
as a recovering IT person, there are two
things I hate. Phone systems and
printers. And printers have turned out
to be a compliance nightmare in most
cases because they send all the jobs in
plain text. And if they transverse the
network that's supposedly not in scope,
guess what? The network comes in scope.
um unless you're using FIPS enabled
printers which are very expensive and
very hard to find as part of that. So
consider you know bringing a USB drive
that's encrypted to the FIPS standard.
Um maybe in lie of printing something
over the network maybe take that USB
plug it into a physical workstation with
an approved USB printer not transversing
the network and think about doing things
that way. And then of course leverage
FIPS 140-2 validate encrypted USBs kind
of like what we talked about
here. All right, before I move on to my
next favorite industry, any questions?
Any manufacturers that are trying to do
an enclave? Hand up over here. I'm so
sorry. Whoever is the question
person, he's coming. The one and only
Jason Sper, everybody.
Oh, stop. They just hit their hundth
podcast episode, by the way, if you're
not a podcast watcher. Uh we're very
very proud of him and Jacob. Fire away.
Uh just question about the printing
again. Sorry about that. Um so you
mentioned the solution was to um use a
USB drive, but you still got to um copy
the data to it. So you're traver
traversing the network. So what we
typically see here, this is a very good
question, is we would call one of these
physical laptops. You see here in the
middle and the bottom we would call that
a staging laptop and that laptop would
be joined to the govcloud. All the data
transversing from there to the gov cloud
is over TLS which meets the encryption
standard. You pull down the data from
the enclave environment, the virtual
environment. You plug in an approved
allow listed USB into that staging
device, copy the files over and then
carry it on over to whatever machine you
need to go
to. Rock and roll. Got some thumbs up.
Anybody else in the manufacturing space?
fire away. Let's Oh, you were just
waving at me. That's okay. It's nice to
see
you. Anybody
else? All
right. Next, we're going to talk about
architectural engineering and
construction. If you would have told me
five years ago, Daniel, the AEC
community would be one of your largest
types of clients that you support, I
would have thought you were crazy. I
thought it was primarily manufacturers
that did all the work for the DoD. Turns
out they're building a lot of things
these days, guys. Um, we heard from John
at Tudaparini. Guam's lighting up like a
Christmas tree right now, right? They're
building all sorts of stuff over there.
We talked to companies that are dredging
things at all sorts of naval ports these
days. And you just wouldn't believe it.
It's kind of crazy. I sometimes tell
people that with the conversations that
we have on a daily basis, it kind of
makes you want to go dig a well and
build a cabin somewhere just in case
because things are getting a little, you
know, too real for comfort, right? All
right. Well, let's talk about AEC
companies. Very similar to manufacturing
and you're also going to see this in
regulated research. Needs to be able to
receive CUI in a compliant manner,
right? Whether that's drawings,
blueprints, schematics, you name it,
right? needs to be able to leverage
again some of the same applications.
AutoCAD, Revit, Solid Works, fill in the
blank. Needs to be able to plot
blueprints or schematics. This one's a
fun one.
Um, a lot of companies will take a
printed file onto a job site uh so that
they can then pass it out to their
subcontractors, right? Doing the work.
They need tablets for job sites to take
pictures, to review drawings, so forth
and so on. This ends up being the more
recommended approach uh that we tell
people. It's like instead of printing
and plotting, try your best to try and
digitize that to some degree. Have your
CUI compliant iPads that are joined and
walk them out to the job sites because
you can also take pictures and upload
them to your one drive, right? Or
shareepoint or teams so they can then go
back into the right repository. Um
things like that, right? All right,
let's get into another pretty picture.
very similar
here. So, considerations in tune for iOS
and Android enrollment for being able to
take pictures of job sites. We talked
about that before. This would be a
really good use to again have these
staging iPads that you're handing out to
subcontractors or to your own
employees. Leveraging a site toVightVPN
connection for pulled licensing servers
for expensive or critical applications.
Guess what? You might have spent
thousands of dollars for some of the
software that you have that's in a
poolled server on prim. Guess what that
pulled license is not? It is not CUI,
which is great. Uh, however, we need to
run that application inside of the
enclave. And to do that, we would do a
sight toVightVPN connection back down on
prim uh to be able to activate our
software so we don't have to buy a
separate pool of licenses running in the
gov cloud. Okay.
Secure a specific room as the physical
print CUI room. So if you do have to
print something, make sure that you're
not bringing your whole facility in
scope and try and just isolated to a
specific room. Ryan Bonner and I have
joked for quite some time, construction
companies need to build an enclave
trailer where they drive it to a job
site, they drop it off, it's got all the
physical protections, it's got the
drawings in it, the iPads for checkout,
all of the fun things. And uh anyways,
you might want to think about a mobile
version of this and then access to the
enclave for your supply chain. You guys
can't do the work without your
suppliers, but your suppliers need to
know what kind of work you need done,
right? In order to even bid a project
most of the time. So, a lot of
organizations are starting to give
access to their to their enclave to
their suppliers just to be able to see
documents and drawings and things like
that. I'm going to pause here for just a
second. I'm gonna sadly just Okay, a lot
of people ask me, Daniel, do you wake up
every morning trying to make people cry?
And I say, I don't mean to make people
cry. It is a byproduct of some of the
things, some of the words that come out
of my mouth.
Um, you cannot do an enclave for all of
your
suppliers and and
they how do I say this? If you built an
enclave, a supplier network enclave,
okay, and you were giving it to a
hundred of your suppliers and they were
using that as their CMMC assessment
scope. So all they had to do is the
maybe the physical controls, but more or
less probably the authorization controls
of who they're allowing, background
checks, things like that. So let's say
you're taking 80% of the burden, they're
having to do 20% for CMMC. And the
assessor right at that point would
assess their 20% and they would treat
you as an MSP that's providing them an
enclave to do the work. Here's a gotcha.
When it comes to your supply chain, if
you build an enclave for them to use and
that enclave is part of their CMMC
certification boundary and they're doing
DoD work with your
competitors, guess what? You don't want
them
using your Enclave. So it's a great idea
in theory that you guys could be able to
offload a lot of the issues of your
supply chain. However, when you look at
the actual certification boundary, it
becomes very complex very quickly
because you're not going to permit them
to do competitive work in your enclave
environment unless you're just really
really nice. most businesses aren't
quite that nice. But um but yeah, it's
just something to really think about
because a lot of people think they can
just build an enclave and outsource it
like an MSP and they can save their
whole supply chain. Uh and you just
can't do
that. All right, before we get into that
question.
Oh, wait. Let's get We're gonna get the
mic. Sorry.
Just so the live stream. Yeah, people
like to hear what you're saying, believe
it or not. I know it's crazy.
Give me a bit of a warning. I'm sorry,
Sper. Sometimes I don't know when my
slides end, so I just kind of keep
clicking until How do you deal with
architecture engineering companies uh
like AutoCAD products are not FIPS
compliant or compatible? Because if you
enable FIPS, it won't work. Uh this
one's tricky. So I'll give you an
example of
this.
QuickBooks. QuickBooks. If you enable
FIPS on anyone tried to enable FIPS on
QuickBooks on prim anybody any takers
did it decide to love you or hate you
decided to hate you right so very
similar when we're kind of going through
this
exercise here's one of the nice things
about it so like the Azure environment
right it all of its hardware is FIPS
validated encrypted already at the drive
level and so that all of the data being
processed on that system on that VM we
can we can check a box on. However, if
you have a physical device, you have to
enable FIPS on for the hardware piece
and then the software piece is part of
that as well. You're going to start
breaking stuff and it's very very
difficult to get around that because you
you're going to have to do it. You
either have to get CUI off of that asset
or you're going to have to figure out
some other workarounds where you can
enable
FIPS. I wish there was a better answer.
Most software
applications just like a lot of cloud
providers didn't know what Fed Ramp was
until CMMC came along a lot of
application vendors haven't realized
what FIPS was and again until a massive
wave of people have basically said hey
your application I'm spending hundreds
or thousands of dollars a year on it and
I can't use it right so one of the
interesting things especially with the
AEC space you guys familiar who's in the
AEC space anybody we got some okay blue
beam right big fan of blue beam All
right. I was talking to a 30 person
construction company and they were like,
"Daniel, you're never going to believe
it." I said, "Please tell me." Because
Blue Beam, for those that don't know, is
not Fed Ramped. It's a major tool used
in the cloud. Um, Blue Beam has a local
install that you can sell and host in
your own enclave.
For the AEC companies, that's really
important because a critical piece of
technology that they use, they haven't
been able to use or they had to descope
all the CUI out of it. Now, you can
self-host it. You have to like go
through like three back doors and knock
twice in order to get it, but it is out
there. So, for those that are familiar
with that, it's definitely worth taking
a note
on.
John, oh, sorry, Sprer. We we got we got
my favorite people. We got Tutaprini and
HDR both raising their hands.
They're gonna have to fight over one
mic. This is the real show, people.
Okay. So, we have um a situation where
uh we needed um remote printing at a in
a secure office at one of our locations.
I've gotten five different answers on
this. So, Oh, I bet you have.
So, we So, we u we print in the enclave
or, you know, we do a print job in the
enclave and we have a printer logic
setup, right? So we have a print server
there. It encrypts FIPS 140 all the way
through to the printer at the remote
site which is a you have to put a code
in at the printer to get your job. So
it's encrypted all the way through. On
top of that from the enclave to that
secure room is um sight to-sightVPN
through firewall and a switch to the
printer and that's all TLS 1.2.
And my question was, is the network is
the firewall and the switch out of scope
because it's encrypted all the way
through FIPS 140 uh to the
printer even though the site to sight
right is you know from from the enclave
to our our location is you know the
sight to sight terminates at the
firewall.
So, I've gotten different answers from
different assessors who are saying yes,
it's out of scope. Others said no, it's
in scope. You ready for my answer? Yes.
Okay. Summit 7 just passed our CMMC
certification. Whoop whoop. Scott
Edwards, thank you so much for having
the foresight to do that. And so, we
have a lot of people that work remotely.
Okay. And so crack open up an old open
an old laptop do some work connect to
the gov cloud and we consider our GCC
high instance and our laptop CUI assets
as part of this exercise and I'm working
at home and I don't have a corporate
firewall at my house and I don't have
any of that but my connection to and
from GCC high is encrypted over TLS same
FIPS validated cryptography that we
talked about and for some reason that
alternate work site policy is more than
sufficient to leave everything else out
of scope.
from my laptop to the cloud and back
down. So when I talk to assessors about
this exact problem, I tell them the
exact same thing. I say if it's
encrypted just like you would treat the
internet connection over TLS 1.2 to the
GovCloud and back down, it's the same
type of concept except we're just
putting it in a different looking
wrapper. That's it. Still FIPS
validated. We're just encrypting it
instead of the TLS HTTPS connection.
we're doing at the print driver level
and it's shipping across the network and
that network because it cannot read the
data. Even NIST actually says if it's
encrypted to FIPS, they don't consider
it plain text. If it's not encrypted to
FIPS, they consider it plain text. And
it's transversing my whole network to a
printer where I will go in and badge in
or release the job through
accounting. And that seems to have stuck
with a lot of people. But this brings up
another good point. Make sure to do a
little bit of speed and blind dating
with your assessors to ask some of these
poignant questions or use a conduit like
myself or someone at Summit 7 to ask
these questions on your behalf. That way
they could come still do your assessment
um because we will try and track down
some answers for you.
Fire away, Dan. Um I have a question
about EOL. So
A and C we do a lot of longterm projects
and a lot of times you start with one
version. So we'll use for instance like
Revit and Revit is every year they put
out a new iteration of it 2025 2024.
Yep. And and they only support back to
back three years prior to the current
version. So you have four given versions
of Revit up at any given time, but that
last one drops off each year when the
new one comes on. Yep. Right.
Um, however, we get into this weird
conundrum where we also have
requirements for our clients, the DoD,
who want us to maintain the records that
we had from that that are no longer
compliant or not compliant, no longer
compatible with the software that we
have advanced to, meaning we have to
essentially keep and maintain. Sure. A
2020 a 2015 Revit version, for example.
for example. Yeah. Right. How do how do
you recommend handling that in the
future? Right now, I think Rev 2 says,
you know, just manage it and so we have
the ability to have a little wiggle room
there. Yep. But I when it we go to Rev
3, it's going to be a completely
different ballgame. There's going to
have to be a level of exemptions from
the DoD CIO would be my recommendation
for stuff like that moving forward in
Rev 3 because CMMC 1.0 level three had
the same problem. they said you just
listen if you can't patch it you gota
got to get it out right um so there's
going to have to be some exceptions
played out when it comes to some of that
stuff because Rev3 is a little bit more
heavy-hitting on those requirements so
my recommendation proactively go to the
DoD CIO for exemptions have that on file
and then show that to your
assessor all right I'm on to my final
one I've got eight minutes left ladies
and gentlemen and then you get to go to
happy hour who's excited for happy
hour regulated research needs to be able
to receive CUI in a compliant manner.
You're seeing a little bit of a common
theme here. Needs to be able to leverage
specific applications to perform the
work. Mat Lab, Python, you name it.
Needs to be able to connect to multiple
research labs. This is fun. Um, needs to
be able to segment non- US persons away
from export control data. A lot of grad
students are not just US persons. A lot
of grad students come from all over the
world to do research. uh and they might
be doing CUI related research that's not
export control, meaning they could be in
the enclave. They just couldn't get to
all of the enclave, right? And we'll
talk about that here in a second. Needs
to be able to carve out charge back to
individual grants, contracts, and
research. Uh I'm not going to I'm not
going to point them out, but I know at
least one university sitting in the room
uh that we've had some of these
conversations with. Uh the CIO's office
does not want to foot the bill for all
the researchers work. We're talking
thousands and thousands and thousands of
dollars, especially when you involve
high performance compute as part of this
as well. So what does an enclave look
for a lot of universities? Leverage
purview site containers and custom
attributes for US or non- US persons in
the tenant. My recommendation especially
if you're a larger enterprise things
like workday or his systems where you
can identify citizenship or personship
ahead of time using that to provision
the accounts inside of active directory
and intra ID and then through dynamic
groups identifying that custom attribute
start putting in site containers and
permissions based on that for specific
sites where there's going to be export
control
data siteto-sightVPN connection to labs
which we'll talk about here in a second
ability to join physical devices to the
gov cloud for local CUI uh access very
similar to manufacturing ability for
chargeback per subscriptions to unique
contracts and grants. So what's
interesting about regulated research? So
we're working with a large research
institute right now that has somewhere
close to about 200 labs. You heard me
right. 2000 uh do you think they're all
managed the exact exactly the same
way? No, they are not managed exactly
the same way. So we want to roll up as
much compliance stuff into the cloud as
possible and limit the physical
protections having to be applied on prim
right asset scoping is very critical in
this and robust adherence to the
physical and authorized user protection
policies are very very very important.
It's the only way that you can succeed.
And I'll say this for all my fun
university friends out there. Uh do not
let a department spin up their own
enclave. It needs to sit somewhere like
the CIO's office. Uh because there needs
to be a high level of oversight because
let me tell you a scary
story. I'll call it a top 10 university
in the United States calls me up one day
and says, "Daniel, we got a problem." I
said, "Oh, that's the first time I heard
that one. Like, we need to do an
enclave." It's like, "That sounds great.
We do those all the time. We turn the
crank, right? Let's do it." He's like,
"Do you know why we need to do an
enclave?" I said, "No clue." He said,
"We just found two high performance
compute on-prem environments that are
doing highly regulated research that we
did not know existed until
yesterday." Do you think that had NIST
171 applied to it? Absolutely
not. Some researcher grad student stuck
it in a closet somewhere with a bunch of
power supplies and called it a day.
Another fun conversation because a lot
of times these contracts and award will
be awarded directly to the
researcher. This is another fun one.
They'll go sign up with their Gmail
account for an AWS commercial
subscription and start doing all their
work. Well, that seems like a problem
because they're haven't implemented any
controls. They're just out there just
doing their thing with zero oversight.
And universities are always afraid to
confront these people because guess
what? they're bringing into the
university dollars they're bringing in
money. So you have this tension with
regulated research where you're inviting
people to do their higher level
education with you but they're bringing
research dollars with them which are
very
enticing. So where's that balance at?
Right? Giving them an environment that
they can play in that will meet their
needs that is also regulated
appropriately. uh it's a lot easier said
than
done. So this is something like a
chargeback model would look. So Azure
similar to AWS and other cloud platforms
has subscription provisioning where you
can provision multiple different types
of subscriptions to have unique
chargebacks. Not only important for
regulated research, it's also important
for other organizations that want to
charge back specific Azure spend to a
specific contract vehicle. Right? So
this is just an example, right? You
might have a top level global
monitoring. Maybe that's where your
Sentinel instance sits for your SIM.
Maybe that's where your AD sits if you
have active directory, so forth and so
on. And then you might have
subscriptions on a per research basis,
per grant basis, so forth and so on. You
know, maybe one of them's 5,000 a month,
2,000 a month, $1,000 a month, whatever
it might
be. Building that architecture on the
front end and scaling that appropriately
is really, really important. doing it
retroactively becomes a little bit
harder, especially if you've not
segmented kind of what I would call your
core back office support elements under
like a global monitoring
subscription. And this looks like a fun
board game to play. This is are you a US
person or not? So this is the fun logic
when we're talking about provisioning of
identities for US persons, non- US
persons. Oh, guess what? You can get
exemptions through TAA, technical
assistance agreements. So there's so
many variables to consider when you're
actually working with non- US persons.
Some export control like naval nuclear
propulsion information requires US
citizens to work on, right? Even a
higher level than personship, right?
Green cards don't cut it anymore. So
when you're going through the
provisioning at the identity level, it
is highly important to make sure no
matter what industry or vertical you're
in that your HR team is in alignment
with the provisioning and onboarding
activities of your IT team and vice
versa because you need to build your
permission structure off of what HR is
telling you this user can and cannot do
based on the type of person they are.
I'm not saying they're a good or bad
person, but depending on, you know,
where their citizenship or personship
lies. Couple more as we go through it.
There's two versions of an enclave.
There's a hosted enclave environment.
This would mean that you're buying a
subscription to someone else's enclave.
And then there's something called a
managed enclave. So, a hosted enclave is
an environment where they own the
hardware. You're buying a per seat,
right? Typically doesn't scale very well
from what we've seen. hard to get your
data out if you end up breaking up with
them. Difficult to extend your boundary
on prim for some of the use cases that
we talked about. And of course, you
can't get away from the good
oldfashioned customer responsibility
matrix as part of this and fed rampant
moderate or fed rampant moderate
equivalency for the hosted enclave
because at this point very likely
they're going to be considered a CSP as
part of this. The other side of the
fence is a manage enclave. This is
something that we do here at Summit 7.
You own the Microsoft GovCloud. you own
the Microsoft Gov Azure subscription.
You inherit Microsoft's SSP, you inherit
Summit 7's customer responsibility
matrix. Um, and you can extend the
boundary and if we ever do have to break
up down the line, guess what? The
environment just keeps on running. You
don't have to do some fancy jumping
through hoops to get your data out if
that ever were to be the case. We see
most organizations wanting to own the
subscriptions because we've all worked
with service partners before. We just
want to make sure it's going to work
out, right? If we I know people that
went to a hosted Enclave solution and it
took them three months to migrate out of
that
environment. It's just kind of crazy,
right? So, when you're doing your
Enclave research, ask them, are you do
you own it all and I just pay you a $100
a user or do I get to own it and have
some level of insight and control over
it?
Right. And it is 4:00.
It says I have 10 seconds left here on
the clock. We had one question. We had
one online question if you have time,
Daniel. Oh yeah, I've got all sorts of
time. It depends on how heavy the
drinkers are in here. I'll make a deal
with everybody. I can I can keep going.
Well, I'll make a deal with everybody.
We'll get through this one question and
then the other ones that came in, we'll
put on the Q&A for next Friday. There we
go. Because you'll be there on the
hotline. So, one of the questions that
came in uh is can Daniel expand on what
he meant when he said that contractor
riskmanaged assets are a damn dirty
trap? Oh,
man. I can cram for those that are
familiar with them are assets that can
sit on the same network as a CUI device
or you know whatever it is um but due to
policies and procedures and so forth and
so on should not be able to process
store and transmit CUI. So, you get into
an assessment, you've got a CUI asset,
boom, on my network, I've got a CRM
asset that shouldn't have CUI on it. And
assessor comes in, looks at my security
policies, and says, you know, I just
don't believe you. It just doesn't look
like it's enough. And then with the cap,
we now have to assess against the 110
controls on that asset. That's a little
problematic because I kind of said it
was a CRMA and I didn't do any of those
things because I thought it wasn't
really going to apply, but now because
you're challenging me on it, you have to
assess it to the 110 and I wasn't
prepared and that assets not compliant
now and I get dinged on my assessment.
That's why CRMAs, in my opinion, are a
little bit of a trap. I don't know
anyone using them well, I will say. Um,
so tread lightly on that. I would stick
with your CUI, your SPAS and your
specialized assets primarily.
And ladies, that is the end of the talk.
It was a pleasure talking to you today.
Daniel Acreage everyone
Hey,
