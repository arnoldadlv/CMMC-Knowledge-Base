---
source: Summit 7
type: youtube-transcript
url: https://www.youtube.com/watch?v=NXXNTo_vGpU
date: January 24, 2026
tags:
  - cmmc
  - dib
  - summit7
---

# CUI Hotline - Weekly Q&A with Ryan Bonner

**Source:** [Summit 7 - YouTube](https://www.youtube.com/watch?v=NXXNTo_vGpU)
**Date:** January 24, 2026
**Guest:** Ryan Bonner (Defcert)

---

## Key Topics Covered

- **CMMC-as-a-Service / Per-Seat Enclaves** - CDO (Customer Documents Only) enclaves, risks of minimal enclave solutions, business process rearchitecting
- **CMMC L2 Required Before RFI** - UAS program requiring L2 attainment just to access RFI details (Linda Rust discovery)
- **Prime/Sub Supply Chain Pressure** - Subs losing work for SPRS scores below 88, primes silently dropping non-compliant vendors, certified subs getting more work
- **10-Minute Assessment Debunked** - Why a legitimate CMMC assessment cannot be done in 10 minutes, pre-assessment evidence review vs live assessment
- **Encrypted CUI Still CUI** - DoD FAQ clarification that encryption does not create logical separation, CUI assets include network transport layers
- **Logical Separation Requires Preventing Data Transfers** - Zero trust browser/device approaches as potential new paradigm
- **Practical Scoping Example** - VDI + FIPS printer + VPN network: all three are CUI assets, but network component only needs 2-3 NIST 800-171 requirements
- **SPRS Minimum Score of 88** - Not all paths to 88 are valid; specific 5-point and 3-point controls must be met per 32 CFR
- **Assessment Costs / No DoD Funding** - DIB historically spending 1% on IT vs 7-8% in regulated industries; no budget for CMMC subsidies; set-asides don't trump CMMC
- **GSA CUI Requirements** - New GSA publication requiring Rev 3, RMF, 1-hour incident response; likely scoped to large contract vehicles; Appendix E vendor documentation guidance
- **Legacy CUI Drawings (25+ years old)** - Ask for CUI category to understand laws/regs behind it; "CUI positions" approach; CDO enclave for legacy docs
- **MSSP/ESP Responsibility Matrices** - MSSP should synthesize all underlying tool CRMs; watch for pass-through services; ensure someone can speak to implementation on assessment day
- **GCC High Encrypted Email** - Email-level encryption (one-time passcode) vs Purview label encryption (cross-cloud B2B required)
- **Security Cameras as CUI Assets** - If camera can capture detailed visual access to CUI on screens, footage becomes CUI; don't point cameras where you wouldn't allow camera phones
- **Paper Copies Loophole** - Impractical for most orgs; requires ALL customers to agree to paper-only; suppliers demanding paper-only will get dropped

---

## Transcript

Hey, we are here and you are not Jacob,
Ryan Bonner. Uh, welcome to CUI Hotline,
one of the most esteemed guests that we
have on the show. Ryan, how the heck are
you, my friend?
>> Pretty good. Pretty good. Fighting the
good fight. We're uh working through a
lot of organizations
uh implementations of CMMC right now and
uh just going with all the you know the
the fun activities that are part of that
uh dealing with constant change.
>> Oh yeah.
>> Uh you know everything from regulatory
input all the way down through how
C3PAOs are interpreting things. Just the
whole gamut. It's it's fantastic.
It's one of those things now that we're
in it, I'm running into like two
different sides of the coin. Believe it
or not, I'm sorting into I don't think
it's going to impact us or we don't need
to be compliant until November 10th of
2026 or you know, something like that.
And then I have the other that's like,
oh my god, we're losing money. Like
they're not giving us work anymore
because our score is less than an 88.
Like there was a story yesterday on the
Discord that was like, "Hey, like we do
work with GDIT and we lost a bunch of
money because we weren't compliant. We
didn't have a score in place, right? And
it's like our score was below 88
>> and they said, "Hey,
>> no, no, thank you. We can't use you guys
anymore." And they had like several
millions more on the line potentially if
they didn't get compliant within like 90
days or something like that. Like, so
it's so interesting to see both sides of
it. It's like the people that are like
naysayers or pushing it out. I'm like,
well, your primes probably aren't
sending you work because they know where
you stand. And then you have other
people that are like, oh, I'm actively
losing dollars out the front door and
like I need something compliant like
ASAP, right? And so, um, that's kind of
leads me to my, uh, weekend review,
which is compliant in 60 days. I've had
multiple phone calls today where it's
like we need to be compliant yesterday,
right? Because we're afraid that any day
our prime could could call and ask for
where we stand in this process. And like
that's a real fear of people, right? Um
and what I'm seeing a lot of maybe you
can fill in some blanks here, Ryan. A
lot of people are going to like the
native cloud hosted
uh per seat license of like an enclave.
like you pay me 200 bucks, you get a
virtual desktop and that's kind of the
end, right? Maybe you get an email
account, you get some office apps, maybe
um we don't get a lot of flexibility to
deploy other things in that environment
and they're like, "Hey, whatever it
takes to get it done fast, but then we
have conversations around like
significant change and what that means
and all of that." So Ryan, for people
that need it fast, that need it
tomorrow,
>> what are the risk of going with
organizations that are offering this
CMMC as a service per seat license? Um
or just what are the things to be aware
of, right? Like what are the goods, the
bads, the uglies when it comes to stuff
like that?
>> Sure. You know, a lot of times we're
trying to almost characterize the
different kinds of environments that you
can set up, right? and and we've started
to build some language around that. Uh
so the the smallest enclave would be
like what we call a CDO enclave,
customer documents only. And that's
where you find a way to like start
piping customer downloads maybe from DoD
safe, maybe from a portal,
>> whatever into that environment and then
for risk of expanding your scope, they
can't really leave. So, it's like a look
but don't touch kind of situation and
and you're doing a lot of read only
access and things like that. Um, it's
definitely like minimum viable product,
>> but you got to keep in mind the the
documents have to get there somehow
correctly. And so sometimes you're
having to reshape information flows or
try to get, you know, specific customers
to start communicating with you
differently or sharing things. you know,
you can't just
>> email the drawing revision to the last
engineer you talked to inside of our
company.
>> Uh you have to go through this new
shared mailbox we set up or whatever it
might be.
>> Yep.
>> And so in in those situations, there can
be a lot of work to do to rearchitect
the the business process. If you ever
heard of like I think it's Conway's law,
right? Like you have to design a system
based on the communications.
>> Like the communication flows should
inform the system design.
>> Otherwise,
>> Conway makes a lot of sense. He's making
a lot of sense.
>> Have a system that no one uses.
>> That's just fair.
>> Yeah. So, I I think uh almost anybody
who's going to look at one of those like
very self-contained
uh environments is is going to
immediately start to have conversations
about well that doesn't match the way
that we do business.
>> Yeah.
>> So, we've got to expand that capability.
So one of the things we're always
looking out for in addition to like how
do we shape data flows is how many knobs
and levers do I have
>> to expand the functionality expand the
user count workloads add applications
whatever it might be and that's really
going to be the the litmus test for
whether a situation like that would work
for you because if you can't install
software if you can't you know visit
more than five websites what whatever
the situation is you just got to be
aware of what those limitations are
going to be. And that probably only
bought you some time to maybe either
move into something bigger and more, you
know, more capable or, you know, figure
out it's not for you.
>> So, we'll we'll ask this as a follow-up
question because I do want your
interpretation of significant change
because that's been such a fluid
conversation when it comes to stuff like
this. But before we do that, Ryan, we
always like to ask other guests their
weekend review. And you were sharing a
very interesting story about CMMC level
two requirement prior to award. Can you
can you tell us a little bit more about
what that is or what you what you saw?
Yeah, a huge shout out to industry
stalwart Linda Rust for pointing this
out to me, but uh she had tracked down a
request for information for the next
phase of sort of like the bake off if
you will for unmanned aerial systems. So
uh these these larger um uh UAS systems,
the next phase of the capability trials
and things like that, in order to even
find out what the defining
characteristics were for this next RFI,
you had to prove that you had CMMC level
two attainment in order to even get
those characteristics documents.
>> Interesting.
>> So you've got a you've got a you know an
all hands- on deck. We'd love to hear
from you. Request for information, but
if you want to know what the request is
in any meaningful detail, uh you've got
to show that you have CUMC level two.
And that's kind of like uh one of these
things where like nature will find a
way. like yeah if
>> collection it's like oh yeah
>> yeah if if you're in an acquisition
command and on the last round of these
RFIs you got way too many respondents
and way too many headaches if you want
to cut down the signal to noise ratio
what better way to do that than to
create a roadblock on the front end for
even participating so wasn't wasn't
expecting that uh as as a possible uh
tool that that CMMC could represent to
program managers, acquisition commands,
individual contracting officers. But
wow, what a what a way to shift left and
use CMMC
uh a as a way to really control
outcomes. Probably won't be the first
time we see that, but it's interesting
to see it so early on in the in the roll
out of CMMC, right? It's like, hey, I'm
a contracting officer. I don't want to
review 10,000 proposals, right? I want
to self- select the people out that I
know aren't going to be able to get it
at time of award and not even work in
that middle part, right? Let's just go
ahead and get ahead of it, you know,
because the other thing on the other
side of this, if we're looking at the
prime level and the sub relationship,
like you work with both primes and subs
all the time, all the day long, are you
seeing any kind of similar requirements
as like a prime? like we had Elbert on
last week or the week before on the
podcast like and they're saying things
like, "Hey, if you're certified, let us
know, but if you're not, we're okay not
working with you anymore." Right. Are
you seeing those conversations play out
on either side of the fence about the
supply chain?
>> Yeah, we are. You know, a lot of our uh
clients are subcontractors, right? And
so they're they're working through
primes. they have usually more than one
prime as their customer and so they're
they're seeing sort of like a spectrum
of responses.
The the folks that I would be worried
about are the ones who just aren't
hearing anything from their customer.
That could mean that they're off of a
vendor list. They're not planning to use
them. They're actively trying to remove
them from a relationship. Uh and you're
just not going to know until it's too
late. They don't have to say anything.
they can just stop calling you, stop
asking you to bid, stop whatever. Uh on
the other side, we're seeing
subcontractors
who are having it like positive
communications from their customers that
like, hey, the reason you are getting
more work right now is because you have
your certification
like very clear linkage between you have
your C, we're going to start to shift
work over to you. And so yeah, we're
seeing a spectrum of responses from uh
those vendors. And then of course you're
also seeing the supply chain risk
management activities of like hey where
are you at? What date will you be done?
And that is really starting to drive
board level topline executive management
discussions on it needs to be done. It
needs to be done by this date
>> and it's not just because we picked that
arbitrarily. We we actively told some of
our biggest sources of revenue that
that's when we'll be done. And so we we
are now starting to see contractors show
up on our doorstep saying this date I
have to be ready on this date.
>> Wow. That's man and there's only so many
I would say competent implementers of
this service and that that backlog we
talk about it all the time like Jacob
and I do like the backlog to get
assessed actually probably isn't is
probably shorter than the backlog to get
into a compliance state prior to
assessment because there just aren't a
lot of parties out there doing it doing
it well right I mean the MSP collective
I think has 20 or 30 in it right that's
obviously not all the eligible parties
but I mean if that's a good sample size
of MSPs that have been certified, you
know, 30 versus 300,000 people in the
DIB, you know, organizations. So, it's
going to be really interesting to kind
of see how that narrative keeps
progressing because, you know, it's like
at some point backlogs are going to
speak. I mean, they're going to be weeks
and months potentially, right? You can
only scale organization so rapidly and
so um yeah, it's the classic like
>> you got to get in line now to get
something a few weeks or a few months
from now, right? So,
Yeah, that's that's a huge
consideration.
>> Hey, uh I think you know this guy Andrew
just shouted out heard there was a
prize. If we could stump Ryan, there is
a $5 bounty on Ryan's head today. If you
can stump Ryan Bonner, I will. PayPal,
Vinmo, or whatever you $5 for your drink
of choice. Um or you can do whatever
you'd like with it. Um so yeah, so get
get the stump stumping going here. So I
think we have our first one. Maybe we
got our first contestant, Nicholas. At
what point are security cameras a CUI
asset? If the resolution and location
elevation is good enough to see general
events, but poor enough that you can't
see anything specific on a computer or
print, is it safe to say it's just a
security protection asset? Ryan, this is
stump chance number one. Nicholas might
be getting five bucks today.
>> Yeah. Yeah. You know, Nicholas, this
this conversation has come up before and
ultimately
here's how we've come to view the
problem, right? Um, when you think about
a video camera that might have the
ability to see a a piece of paper or a
computer screen, really what it just
comes down to is whether or not that
recorded video footage would allow you
to, you know, zoom in, sit on the screen
that was captured in that footage and
derive information, derive knowledge
from what you're seeing on this the
screen to the point where now you know
how to produce or reverse engineer or
continue the design intent of something
that is uh controlled information,
controlled unclassified information. And
so really this comes down to uh just an
understanding of what what are like the
sustained uh coverage areas of these
cameras and things like that. the the
simplest and best rule that I've seen
put forward by members of our team, some
of whom have developed very robust like
ITAR compliance programs inside of mega
primes, is that you should not point a
video camera at anything that represents
an area where you also would not allow a
camera phone or someone to record
footage or take pictures or anything
like that. If you're not comfortable
with someone walking up to a computer
and like holding a phone up to it and
recording video or taking a screenshot,
it probably shouldn't be in in range of
a video camera either. And so that
creates uh at least not without the
video camera and its footage becoming
cui if that tracks. So, uh that could
drive some really strategic
conversations on where do you want video
camera footage, right?
>> Perimeter entry exit points probably an
awesome idea. uh major, you know,
barriers or or or passage points in a
building? Absolutely. Probably in key
safety areas, loading docks, probably
fine. But do you want them in the
engineer cubicle pit? Uh
>> I'm not sure about that one. That that
that could create some additional
issues. So, you know, that that's how we
tend to think about those those um
challenges. If you want a really good
example of this, uh, look at like how,
um, the Department of the Navy describes
the difference between like casual
access and what's called detailed visual
access. When you're you're talking about
export control, naval nuclear propulsion
information or things like that. Um, if
if I have the ability to study and
derive knowledge from something, it's a
problem.
>> Okay. I would say stump chance number
one, you have conquered, Ryan. Uh, this
one's going to be interesting. This is a
hot take from the co-star of CUI
hotline, Jacob Horn, who's on travel
today. Jacob, hope you are traveling
safely, my friend. Uh, LinkedIn hottake.
Today we saw a LinkedIn post saying and
celebrating, I believe it was an
11minute CMMC assessment is is how long
it took before their assessment was
complete. And so obviously that sparked
quite a few conversations already. Um,
and so Jacob's question to you, Ryan, is
it possible to complete a CMMC
assessment in 10 or 11 minutes or less?
>> Uh, no. Uh, not not as not as prescribed
by the CMMC assessment, uh, like
process, uh, the CAP itself. Um, even
just like any durable concept of like
completeness or assessor confidence or
like anything that you would like you
just literally the human brain cannot
process the information fast enough to
comprehend 320 assessment objectives in
10 minutes. Um, unless you're you know
you taking that that pill from
Limitless. But like the here's what I
think is happening in the situation. I
I'm not directly familiar with this.
Okay.
>> So, someone else can weigh in if we they
think it's different. Here's what I
think is happening with this. People
look at the amount of time that uh a
lead CCA or lead assessor working for a
C3PAO
takes in their, you know, during their
window of their scheduled assessment and
they say that's how long the assessment
took. You know, we have organizations
who have basically wrapped an entire
level two assessment in a day.
But the reality is that the only way
that you got that small of a time window
for the assessment is because you laid
out usually visual evidence of how you
met all 320 objectives in a self
assessment that you submitted to the
C3PAO and you gave that to them with
enough
uh time to read ahead and arrive at most
of their conclusions from high
confidence documented evidence. So then
by the time you get to the live
assessment,
you're only looking at the things you
didn't understand, the areas where you'd
like a demonstration, maybe physical
walk through some of the the physical
security things that uh your confidence
meter as an assessor isn't filled up all
the way until you do those things. And
so uh it's a I think in a lot of cases
it's a mischaracterization to say, "Ah,
this only took a day." No, no. It took
two weeks of someone locking themselves
in a in a basement somewhere and reading
through everything and writing met not
met findings
like in a bespoke effort and then they
just showed up to back clean up on
whatever was left over.
That being said, even if that was the
case, if pristine fully understood
evidence was laid out to the C3PO in
advance,
I still have plenty to talk about that
is going to take more than 10 minutes.
it's still a herculean effort to get it
done in an eight eight and a half hour
workday. Uh, a lot of times that will
spill over into additional days,
especially if clarification is needed or
the right person isn't available to
answer a question. A 10-minute
assessment effectively means no
demonstrations were provided.
If there was a physical walkthrough, it
was not counted
>> uh in in that in that elapsed time.
Someone stopped the stopwatch too early.
Uh and and so like it just sort of like
that that sort of is confounding to me
that you you say that you could have a
10-minute assessment.
>> It's an interesting flex too, right?
Because it's also on the other side it's
like and listen I if this if these
individuals are watching like this is
not a jab but it's also like man like
that doesn't seem right. Like it sounds
like some maybe something you wouldn't
want to promote, right? It's like
because the due diligence and the
thoroughess of the assessment feels like
it could come into question it being
just that short. Right. Um anyways, all
that to say is no matter how long or
short, just do it right. Right. If
you're able to somehow do it in 11
minutes and there's high confidence
behind it and you can show your work,
that's one thing. Um, but realistically
after we've gone through now 74 client
certifications, I can tell you right now
10 minutes is nowhere on the radar when
it comes to incorporating external
service providers and interviews,
physical walkthroughs, right? Even if
you're just doing a cloudnative enclave,
there's still so many more things on the
perimeter that have to have some sort of
active conversation, right? So, um, very
interesting. All right, let's keep
moving. I'm going to pivot to one of my
questions and Vincent actually asked
this last week. So Vincent, this is a
follow-up to your yours. Um, DoD FAQs
have been making the rounds the past few
weeks and encryption is not enough for
logical separation of network or like
you have to have both logical and
encryption
now, right? Encryption does not negate
the need for logical separation. I think
I worded this a little poorly, but um
Ryan, what's your hot take on that? Is
that a CUI asset? Because encrypted CUI
is CUI as well. So like how much of my
environment is now in scope based on one
DOD FAQ update?
>> Yeah. And and before I answer this, I
just want to encourage people not to get
stuck in like a false dichotomy where
like being in scope as a cui asset
equals bad and being completely out of
scope is the only good
in in reality not enough people are
going through the process of determining
for an inscope asset how many
requirements would actually need to be
met. And so I think that's the missing
piece that would help stitch back
together some of these seemingly
divisive determinations from DoD. But
yeah, at its core, the DoD uh FAQs
recently have clarified that encrypted
CUI remains CUI, which means just at
face value, anything that's transmitting
or routing or forwarding those encrypted
packets are still a CUI asset, which is
uh a revelation for people in some
cases. And so, um, I think a lot of
people had looked at encryption as sort
of like the cure all for their scoping
woes. Um, including just like if I
encrypt the information, then I've
somehow uh created the logical
separation needed for uh certain things
to be out of scope. I think the reality
is that if if you look at the definition
of an inscope asset and an out of scope
asset in the CMMC scoping guidance, uh
you don't get to say something is out of
scope unless you can prevent data
transfers. So if we're just sort of
combining terms here, right? uh a file
or a data packet that's encrypted but
still CUI moving to another device over
a network did not it didn't prevent a
data transfer
>> right
>> and I think that's that's the part that
people are starting to like come to
grips with and so really in order to
achieve logical separation you need to
prevent transfers right so you need some
way to stop the data from moving from
asset A to asset B if you can do that
now you're in business. I think what's
cool as people go through and understand
this better is that logical separation
is uh the criteria that make something
out of scope. So I think in a lot of
cases we've been trying to achieve maybe
like a contractor riskmanaged asset
status for something that's like on the
same network for example as a cui asset.
If I can stop data transfers altogether
>> like that's the end of the discussion.
So that's really powerful and really
encouraging. I think organizations who
start to look at ways to uh prevent data
transfers could actually reduce scope
altogether in some areas that would be
really compelling. Um, I'm personally
really interested to see if if we can
drive
new um, paradigms, if you will, where
the external boundary in some cases for
my environment is the machine and the
internal boundaries are applications and
file directories. And if I can stop data
transfers in that killbox, uh my new
external boundary might be an individual
device or something like that. That that
could be really cool in a very like zero
trusty
>> application. It sounds like a zero trust
browser like managed browser solution
potentially. Yeah, brow zero trust uh
configured browsers and devices uh that
that are preventing those transfers in
some way uh could potentially mean that
two computers sitting next to each other
on the same network have totally
different asset determinations because
of how they they handle whether data can
leave and where it can go. So really
fascinating and and and um hopefully
promising ways for us to look at this
this new normal. But if we stay in our
old mental mode, yeah, this feels like
doomsday, right? Because like all of
your options feel like they're being
taken away.
>> So to clarify one more, I'm going to
give an actual example because this
comes up quite a bit. I have a virtual
desktop environment running in the
cloud. Well, God bless it. I've tried so
hard to eliminate printing, but but man,
the people love to print, right? So one
of the ways people do that is a sight
toightVPN. that's connecting over the
local network. Now, I've had forethought
to buy a FIPS validated printer. So, the
actual print job is wrapped in a FIPS
validated encryption and then it's being
shot over the VPN tunnel over my
corporate network which I thought was
out of scope previously and then
delivered to a printer in a secured room
that I've had meet all the CMMC
requirements. So with this new
interpretation, just to give a little
bit more of a practical example, that
network is now in scope up to what point
would you call it a security protection
asset? Would you call it a CUI asset?
Would you apply relevant controls? Or
how would you apply all CUI controls?
Help me with like one of those kind of
use cases there.
>> Yeah. Yeah. And I think this is where
you have to shift the mindset from like
CUI asset equals bad and I have to do
all the work all the time, meet
everything everywhere all at once to an
applications
in order to meet the necessary
requirements. So to answer your
question, we've got really kind of three
unique component types, right? We've got
the VDI or the Azure virtual desktop or
whatever it might be. We've got the
printer and then we've got the network
in between.
>> Based on the FAQs and and other factors,
all three of those are CUI assets.
>> So, to me, the real art versus science
of this is like, well, okay, but how how
many requirements would I need to meet
on a network transport layer that is
really just piping previously encrypted
packets between these two components? So
if if I've got encrypted packets that
were properly wrapped and encapsulated
by a FIPS validated module in that AVD
server pool or whatever.
>> Right. And I'm routing those through my
network.
>> I should really only have like two
three 81 171 requirements that I would
need to apply to that network component.
Like the ones that I have in mind would
be like uh number one 31311
FIPS validated encryption.
>> But I have great news. I'm not decryting
or proxying those packets in any way. I
get to inherit that requirement from the
AVD pool that wrapped those packets
before they got to me. So that's that's
awesome.
>> Uh the other one that comes to mind is
31310 key management. So if I have that
requirement to establish and manage
cryptographic keys, I have almost like
an anti- requirement for my network
component, which is under no
circumstances must you give this network
component the decryption keys necessary
to unwrap those those data packets,
which I don't know how you would really
do that anyways. Uh but
great news, I I'm not giving it the
decryption keys. That requirement is
satisfied for that component.
The only other things that I could think
of would be like the 31316 requirement
to protect data at rest and that that
sort of like translates into an indirect
requirement which would be like hey man
don't do packet capture on these things.
>> Like don't don't like do a network
capture session and then sit there with
all this data that could then maybe be
decrypted later. But even that like I
could still argue that that's not even
applicable. So,
is it really that bad for these network
components to be in scope? I would say
like the bulk of the work that you're
going to do is the full featured
operating system that's at one end of
that that piped traffic and then things
like the physical security of that
printer and a few other things you'd
still want to have in place for the
printer itself. So, you know, this is
where organizations who
can get through the like, you know, the
stages of grief and loss and be like,
okay, I have CUI assets, you know, let's
get to the bargaining phase, man. Let's
>> let's start to figure out how many or
how few requirements uh I might need to
meet and have a much more targeted
implementation that I can get through
faster
>> because I think people just immediately
hear CUI ass and they think 110 320.
It's like well if you frame it correctly
and understand the data flow and what's
happening each step it's actually maybe
not as painful as you think it is.
Right? So for those that are worried
about that uh Ryan Bonner owns a company
called Defert. They are happy to uh to
help you in any form or fashion uh help
the scope and the burden of what that
actually looks like. So we don't have
Ryan on here to pitch sales things but
man when you're that good people always
want to talk to you Bonner. So um all
right firing up another question. So
far, I haven't heard of Stump Ryan,
although there is a trivia question from
Vincent we'll have to get here at the
very end. Um, who can should we share
our SPS cyber report with if they ask
DoD contracting officers, primes? This
is the report that is generated by Pie.
So Ryan, you're you're not a lawyer. I'm
not a lawyer. Sometimes we pretend on
the trade compliance side, but even
that's a little shaky. So what would be
your general recommendation for at user
UI5SE 5JV7Q
um for who to share and when to share
their SPRS score with
>> you know I I think one thing to keep in
mind user UI5 SC5 J is that like DoD
acquisition personnel have the ability
to access your SPS score in PIE in SPSS.
already. Um, if they are asking you for
that information,
um, it's because they just want you to
do their job for them. Uh, they can get
access to that information. Uh, if you
feel that there's an advantage to
communicating your score in in a bid
response or to remind them of the fact
that you are eminently able to take a
contract,
go with God. That's fantastic. like you
should absolutely leverage and weaponize
your compliance status into awards and
even advocate for it to be a technical
evaluation factor on a contract. Um,
when it comes to lateral communication
with other people in the private sector,
you know, that's really going to come
down to the nature of the business
relationship, the non-disclosure
agreements you have in place, all that
good stuff. Um, I would say again if you
have an SPRS score that is suitable, an
88 or higher, let's say, and all of your
five-pointers are met and all of your
three-pointers are met, uh, you know,
it's your prerogative to decide if you
want to take a screenshot of that or
something like that and share it with
business partners. Um, that's part of
supply chain risk management. There's
nothing you're not doing anything wrong
by doing that. But, you know, you do
want to identify that the individuals
you're sharing that with uh understand
what it represents
>> and understand that it it is a
competitive advantage for you as well.
So, you know, I would make sure that
you're covered under NDA almost to the
point of treating that as as like a
trade secret. Daniel, you and I have
talked about this before. We know plenty
of contractors who are very quiet about
their level two certification because
they would love for their near peers and
competitors to not prioritize this.
So, you need to know what your corporate
strategy is for leveraging your
certification or leveraging your SPS
attainment to determine whether or not
you would ever want that to be shared
with competitors to have them realize
how far behind they are because there's
a lot of people out there whose core
strategy around that high SPRS score is
to become a sole supplier for as long as
possible.
So man, another stump free Ryan because
that's the thing. People can't reverse
engineer what controls you have met or
unmet, right? Unless it's a negative 203
and a 110 like they they can't figure
out the in between of what's going on
there. So the general risk is fairly
light I would say personally by giving
somebody your score. However, this is
coming up more and more. Actually, Ryan,
I'm going to share my screen because you
know me, I'm a big PowerPointer. Um
minimum score. So you mentioned 88 as
the minimum score, right? And just for
everyone that's on the live stream, like
it's really good to understand, and I'm
going to zoom in here just a little bit
because the data is super small. So this
is straight from 32 CFR, but what this
is saying is like, hey, the minimum
score you can have is 88. There's some
requirements around five and three-point
controls that you can't have, and
there's even some onepoint controls that
you can't have in there, right, that
have to be put in place. So, one of the
things I encourage people on is like,
yes, is the minimum score 88?
Absolutely. The problem is there are
several ways to get to that 88 number
and some of the ways you might be
getting to it are actually not compliant
and you're misrepresenting your
conditional status of CMMC to the prime
or to the DoD. So if you get the if
someone calls you up and says prove it
and you're and you start submitting the
controls that you have met and they
don't align with the requirements of
CMMC minimum scoring that's problematic,
right? Because I know a lot of people
right now that will come to me and say,
"Daniel, I I was able to submit an ADA."
I said, "Great. How did you get there?"
And they start listing their controls
and I'm like, "Yep, not applicable. Like
it doesn't work." Because the DoD
assessment methodology workbook that the
DoD's had for years now, it doesn't have
this minimum scoring column in there,
right? You just kind of have to know it,
right? You have to look at 32 CFR, you
have to look at the cap um to really
figure out what that actually is. So,
just fair warning to everybody, if you
put an 88, it does matter the way that
you got to that 88. And if it's not the
right way, you're again, not to go super
dramatic, but you open yourself up for
potential false claims and all sorts of
fun stuff if you're submitting it and
misrepresenting your posture there,
right? So, um, okay, that that's a fun
one. I've got a followup from Mitch
here. A little bit different topic, but
always fun to talk about. Mitch, do you
think anything will be done to regulate
or limit assessment cost? and does the
DoD or Primes have any resources or or
any or even obligation to help the
smaller manufacturers who can't afford
the high cost? So, the short answer to
that is no. The budget's been the
proposed budget for DoD's been
submitted, right? People are taking a
look at it. They want $1.5 trillion. You
know what's not in that? Funding for
businesses to achieve CMMC, right? I
mean, there was conversations around
potential tax breaks a year or so ago
that I heard people trying to lobby to
help offset some of that or recoup some
of that. Um, but right now the the DoD
is not obligated uh to do that, right?
They have targets to hit for like small
businesses, right? SBA kind of targets.
They want to see small businesses thrive
in the DoD ecosystem, but if they can't
find businesses that meet the
requirements, they're not bound by that
obligation. So being a set aside doesn't
trump CMMC requirements. And a lot of
people think it does. And you know, I
know people in hub zones, minority,
veteranowned, disable, I mean, you name
it. and they're like, "Oh, I think I'll
it'll be a lesser requirement or because
the DoD has a quotota to fill for my
type of business, um, they're not going
to apply or let me, you know, pass
through on CMMC." And sadly, CMMC comes
before the status of your set aside,
right? When they're looking and vetting
things. So, the DoD is not obligated to
write checks to get you there. It's the
cost of doing business with the DoD,
right? and they see it as if you want to
work with us, you got to meet this
requirement before you can work with us,
right? Um Ryan, any hot takes on that?
>> Uh yeah, I just I think it's unfortunate
that there was this fog of war around
how much implementing 8171 was going to
cost for so many years, right? Uh there
wasn't a lot of good research on that.
There certainly weren't any published
numbers from uh regulators, right? And
so when C3PAO assessments started to
become a thing and pricing was being
given to organizations and you start to
see these ranges, it was the first time
that people could attach a price tag to
the overall effort.
>> What you're not seeing though is the the
much much larger price tag of
implementing this 800171.
And so, you know, a couple of data
points that I would look at at least
when the FARC cui rule was released,
they had cost analysis for what they
they thought it would take for a um a
non-federal organization to implement uh
requirements for uh you know,
safeguarding cui on their side. And like
don't get me wrong, it's it's the way
government estimates a lot of these
things is not the way that you would
actually implement this, but they were
easily hitting a million dollars in
implementation. Like just no problem.
And if it's a cloud, even worse.
And so granted, you have to dial a lot
of that way back down to strip out some
of the RMF requirements and things like
that, but like whatever dial you apply
to that, that's still a much bigger
number than what we're talking about for
the costs of assessment. So the other
thing that I would point out is there's
a lot of good research done on how much
specific industries spend on IT and
security as a percentage of revenue. Um,
guess who doesn't spend a lot on it as a
percentage of revenue? Manufacturing and
construction.
>> We're talking like 1% of revenue.
>> But when you go look at heavily
regulated industries like healthcare,
finance, insurance, they're spending
seven or eight% of revenue
>> on IT and security as a as a you know
subordinate amount.
>> So
>> if you are spending 0.2% 2% of revenue
on it and you're and you're worried
about the cost of an assessment, just
know you are now the most heavily
regulated industry on the planet.
>> If you're in the DIB, so you don't need
just a strategy to pay for the
assessment. You need a strategy to re
recompose the entire organization around
some of these new costs and and have a
strategy to pay for that.
>> Yeah, there was a a presentation I did.
I haven't updated this in probably a
year. Um, but it was how to budget for
CMMC and we were looking at like other
regulated industries, right? And you
know the average spend across those and
basically what we anticipate the DIB now
having to potentially offset, right? And
so kind of agnostic of industry, right?
manufacturing, construction, if you're
doing defense work and the burden of
CMMC. Now, scope in this presentation
says a lot, right? Because scope
controls cost as Ryan says multiple
times, but I mean you could potentially
be sitting to 5 to 8% here potentially,
right? Depending on the scope and
historically it's been around 1% maybe
2%, right? And so, um, it is a question
that gets brought up a lot. CMMC raised
the co raised the awareness of the
burden of NIST 8001 171 implementation
as we all know probably listening that
burden's actually been around since 2017
even prior right that was just the
deadline so that's kind of the shakeup
here is that it's a little bit of
whiplash because you're getting a number
that you should have seen and kind of
better understood back in 2017 for the
implementation and then add 40 50
$60,000 now with CMMC level two um and
it's like Oh, like you know spending
300,000 or 200,000 or 100,000 in 2017 or
in spreading out that cost over the
years. Now you're hit with all of that
at one time in a very short timeline. So
now you're going to pay an expedite fee
in a lot of cases to try and jump to the
front of the line so you don't lose
work. So now it's even more of a of a
burden than if you would have done it
potentially in years past, right? So um
it gets gets really interesting there.
So B, here's another one. I don't think
this is a stumper because this is pretty
new information to everybody and I've
seen this comment twice here in the live
stream and I had it queued up as my own
personal question to you. Uh Ian,
longtime uh friend here, do we have any
information on when the new GSA CUI
rules will be applied at award? If so,
when how? And then we had another one
from earlier in the call um talking
about give us a take on GSA situation.
RMF 171 rev 3 1 hour response time. Oh
me, oh my. And so for those unaware,
Jacob uh and I did a podcast earlier in
the week about this random new GSA
requirement that's actually been around
since 2022, but they updated the
document here last week or a couple
weeks ago. I think it was January 5th,
maybe. I could be making that date up,
but early January. And all of a sudden,
it says, "Hey, if you're doing CUI on
non-federal systems, do all those
things. rev 3, RMF, one hour response
time on a potential incident, right? Um,
and and get audited or assessed by a
3PAO or an independent approved
assessor. And so they kind of took a
little bit of all the good things of
CMMC and then overlaid some confusing
things on top of it. Um, and as far as
we can tell, it's in effect right now.
Like there was not there's no rollout
date. There's no, hey, now's the time.
Um, it's supposedly been in effect, the
original since 2022 because we there
wasn't like an effective date there
either. So, I have never run into any
organization that has seen this
requirement. Ryan, I'm curious on your
take of what you know about the GSA
publication of, you know, 45 pages or
so. Um, and also, have you run into
anybody historically saying, I've got to
meet these CUI GSA requirements?
>> Yes. So far everything that we've seen
when it comes to GSA are generally
writein requirements on like very large
contract vehicles. So like stars 3 or
something like that where um you know
the requirements are contained within
that massive spending pool you know tens
of billions of dollars that are going to
be spent on some very specific things
kind of in tanches. So I I don't know
enough about the constraints or limits
of how requirements are incorporated
into these larger GSA schedules or these
larger GSA contract vehicles. So it'd be
irresponsible for me to say like here's
how the cookie is going to crumble. But
things to think about um everything
we've seen in the past has been based on
a particular contract vehicle or a
particular GSA schedule for how it's
going to be included. And I I didn't see
the GSA requirement structured as a
contract clause. And so I I would expect
we'd have to look for the inclusion of
of this requirement in the list of
things you have to adhere to for like a
very specific GSA opportunity or to
remain on a certain schedule or to be an
eligible awardee uh for a very large
like Idiq or something like that. So
again, we're kind of like right back
where we started with CMMC. We'll just
have to keep our ear to the ground and
try to figure out when this starts
popping up. So like literally in
including this uh uniquely named
requirement in your control F search
terms on an opportunity would be very
good to pay attention to. Um, as far as
like the 1 hour requirement and things
like that, this very much feels like uh
a set of requirements that were written
for uh the purchase of cloud services.
Um, that's where I would expect to see
like one hour notification.
>> Somebody posted that it's like bed ramp
requirement is a one-hour response,
right? So it's like they're pulling this
they didn't come up with this number out
of thin air, right? So
>> yeah. So, you know, it would be
unfortunate if that requirement was
applied to uh less critical acquisitions
by GSA, but you know, stranger things
have happened. If you do go full court
with this, then you're going to find
yourself in a situation where people
have no time to even process the
telemetry that they're getting. So,
they're just going to just dump an inbox
somewhere with every alert they get and
say, "You guys sift through it. I had an
hour."
Yeah,
I had an hour. I did the thing. You
know, it's like, oh man, it's
interesting like the burden of CMMC and
then people like, oh, thank God. And
hoping for reciprocity with other
agencies and then GSA is like, oh,
psych, we're going to throw some more
stuff at you. some honestly at the end
of the day I can't wait for FRACUI to
hopefully encapsulate
all of this and just apply it peanut
butter spread agency across all agencies
because everyone left to their own
devices um are just it's kind of wild
west out there it feels like sometimes
with some of these requirements and
thrown around. So
>> now I I will say in that GSA document
there is
>> what I would say is is the equivalent of
like a Dean Martin roast of vendor
documentation that I think everyone
should take a look at. So uh there's
multiple appendices to that document.
Appendix E is guidance on how to write a
response to a security requirement
>> and it lays out in great detail what you
should focus on. But oh man, the please
don't do this list is chef's kiss. Don't
repeat or rephrase the security
requirement instead of answering how
it's implemented.
Yes. Uh don't use boilerplate text.
Don't leave blank areas. Don't just mark
NA. Do not use empty words like world
class user friendly.
>> Oh man, it's you need to check it out
because
>> Okay, I haven't read that bar. That
sounds amazing.
>> Yeah. Anybody here that's ever had to
evaluate technologies, uh, you know,
you're just your soul leaves your body
when you have to read vendor
documentation that's written like that.
And man, it would be so much better if
we didn't have to. So, good on GSA for
taking that off the the playing field.
>> Thank you, GSA.
All right, we're up for a technical one.
Uh, best way to send encrypted emails in
GCC High. So, there's a couple ways to
do it. As everyone probably knows,
there's I can encrypt the file with a
purview label or I can do native
encryption on the actual email as well.
So like what do I exactly do here?
What's the experience? Well, if you
encrypt an email, then once that email
is sent, they get a one-time passcode.
If they're in a nonGCC high, they have
to type in the passcode, the numeric
sequence, and then they get that email
released. Right. On the other side, if
I'm doing perview and applying a label
at a file level, uh this is actually a
newer capability. If I have the
crosscloud B2B functionality set up with
the tenant, um it will actually honor
that label even though it's coming from
a GovCloud. Uh versus before they just
couldn't open that, right? So, if that
crosscloud wasn't set up, they couldn't
open that Excel file, that PDF, that
Word document, um, because it couldn't
authenticate that user base and the
label didn't know if I can't talk to
anybody to authenticate because this
guest user isn't really friendly, um,
that I'm just going to block access,
right? Kind of deny by default. So,
there's a couple of ways to do it. The
easiest way is probably just to encrypt
the email base because again unless you
have more sophistication in your
environment like B2B setup. Um it's
going to be a fairly poor experience
trying to do file level encryption uh
with the need for collaboration and
access. Right? So um that's the answer
there. Follow-up question here. Uh
non-technical. We're going to take a
different turn. Uh Ryan, I always like a
good hot take. Ryan or Jacob and I have
talked about the paper copies
all for a few weeks now. Um, I have seen
I actually heard audible laughter from
people saying, "Yeah, our subsync we're
going to send them paper copies." Um,
and by the way, they're not. Um, so
Ryan, any quick take on this? Paper
copies don't, if you send a paper copy,
for those unaware, based on the DoD FAQs
that came out, uh, you do not have to
flow down CMMC requirements. If the
paper copy never gets into an
information system which they're deeming
a technical type system like a piece of
software, a computer, you take a picture
of it, so forth and so on. So, um, Ryan,
give give us your hot take here. We
won't burn too much time on it, but I
had to just because it's funny at this
point. So, yeah, I I'm not going to get
into like any of the implications of
this dig down in the weeds on the
implementation side, but just think
about this for a second. If if you are
an organization who thinks that you're
going to be able to take advantage of a
paper only implementation, sit down and
like make a list of all of your
customers and ask yourself, am I going
to get every single customer who sends
me FARD defa space contracts
to agree to only communicate with me in
paper and to do that consistently
every single single customer because
forget the hot hand fallacy for a
second. Just because you get even like
one customer to agree to that does not
mean all of them are going to agree to
that.
>> I also just want you to flip the script
on that. Imagine you're in procurement
or purchasing for one of your customers
and you are told by one of your
suppliers, not asked, told going
forward, you have to send everything to
me in paper.
The level of attention that would
suddenly be applied to you as a supplier
would be like the eye of Sauron just
like turning its gaze to like I'm sorry
who is this? I I must not email you
anything. I must not send you links. I
have to print things out on a plotter
and send them to you with the parts. Who
is this? Get them out of my supply
chain. Like doesn't matter how good of a
relationship you have with Sally in
purchasing like this is going to go over
Sally so quickly
>> that like I can't imagine you would last
long in that type of situation. So you
better have
>> some magical special sauce that
literally no one else in the world can
provide and maybe then you can play that
card.
>> Man, couldn't have said any better
myself, Ryan. It's it's hopeful. It's
wishful thinking, right? And everyone
needs a little bit of hope in their day.
I get it. Uh but there's not really any
silver lining with this one, sadly. So,
um Nicholas is spinning the hits today.
Uh what is the best way to manage
employees who are local admins to
support downloading approved software?
Do they need to have a local and general
user account
or let's say a privileged and a
non-privileged account in in the world
that we live in, right? Um Ryan, hot
take here.
Uh I I don't have any crazy takes on
this. Um I would just say that by and
large uh we don't see a lot of
organizations having someone's daily
driver account have the ability to
install its own software. So like it
just kind of is the local admin. We're
usually seeing something else take
place, right? Um you know Daniel, your
team would be way more familiar with
this
>> than me, but we're seeing pretty
broad-based adoption of local admin
password solution. lapse
>> in Windows in particular. Uh you can
even manage that through intoune now. So
you know the the local user does not
need to know
>> passwords. Yeah.
>> Yeah. So you're still going to
authenticate using that second account.
It's going to rotate the password as
soon as you're done. Uh there's no
reason to have persistent privilege
sitting on that daily driver account.
That's what attackers want. Y
>> So don't don't give them what they want.
>> Don't give them what they want. Good
security and good compliance.
All right. This one seems cui uh Ryan,
your favorite topic. A customer has
recently requested that legacy program
drawings issued approximately 25 years
ago, which by the way is 2001.
So I'm old when I have to say things
like that. That's 25 years ago. It's
2001. Anyways, uh none of which are
marked as CUI, but treated as CUI. Is
this determination valid? And on what
basis? So this is precui program
existed. 2001 the CI program did not
exist in the form that we see it.
Obviously, everyone was kind of doing
wild west stuff, DoD DRO statements, uh
F or FUO, right? Um so what is the
approach that they should take? Should
they treat it like CUI? Is there any
law, regulation
or governmentwide policy they should be
aware of? Um help us fill in some blanks
here, Ryan.
Yeah, I I think keying in on law and
regulation could be really important
here because if something isn't marked
as CUI, you don't know the CUI category.
>> If you don't know the CUI category, you
don't know the laws and regulations that
sit behind that category. If you don't
know those, you don't know whether
you're doing crime when you do what you
do with that document. So, if we're
going to honor lawful government
purpose, I need one piece of information
at a minimum from someone who says,
"Treat this as cui." And that piece of
information is cool. What category of
cui?
Because this category is a $1,000 fine
in a misdemeanor. This category is 30
years in a federal penitentiary. I need
to know the category. And the reason
that I would fall, you know, a foul of
those laws and regulations is because
I'm not exercising lawful government
purpose. So it's crucial that we
understand that. So when we talk through
this with organizations handling CUI, a
lot of times we are trying to build a
logical container that the organization
can operate inside of. So like the first
question I would ask is this 25y old
drawing, how useful is it to your
organization? Does it need to go
anywhere once you get it? Is it need to
be broken down for you know subordinate
details and shifted into other formats
and things like that or can you treat it
as an EPA brownfield as toxic keep it
where it's at look don't touch kind of
that customer documents only approach
that I mentioned
>> depending on your usefulness of that
document how much utility it has inside
of your organization
we have seen organizations that say if
you tell me to treat it as cui I am not
saying it is cui but what I will do is
extend it all of the safeguarding
precautions that I would extend to CUI.
So this ends up uh with organizations
adopting what we call CUI positions. M
>> we will apply NIST 8171
to the following kinds of information
and that could include legacy marks
documents when certain markings are
present or when the customer says treat
as CUI where that starts to become uh
less viable is when you do legitimately
need to move that document around
through a lot of different systems
potentially contaminating those systems
and adding 8171 requirements and you
still don't know the CUI category.
So that can be critical. We always
advocate for asking what category of CUI
the customer thinks it would be because
then at least I have the alternative of
saying, okay, I'll go read those laws
and regs and figure out how much of this
25y old drawing is actually subject to
that law regulation.
>> Man, good answers. No one's stumping you
yet. I'm keeping my $5 today, Ryan. We
haven't gotten to the trivia question at
the end, but right now we're doing we're
doing pretty good here. All right,
J78K4K.
Man, we need to work on some naming
nomenclatures here on the CUI hotline.
Um, if an MSSP deploys and manages their
security stack, so let's say they're
using CrowdStrike, we'll use an actual
name for a second to an OSC system,
organization seeking certification. Can
the OSC just use the MSSP CRM customer
responsibility matrix or will the OSC
need to identify ESPs external service
providers in the security stack and get
CRM for that as well? So, I'm going to
explain this for some. So, first off,
good on you for the acronyms because you
I can obviously tell you know what
you're talking about because you're
speaking in the language of CMMC. Um,
for those that don't know, to rephrase
this question a little bit differently,
I am company ABC.
I use an MSSP called Secure Now. Let's
say Secure Now uses Crowd Strike as
their agent that they deploy to do the
monitoring. So the question is, if I'm
company ABC, can I just inherit the
customer responsibility matrix from the
MSSP or do I have to go out to each of
the tools that they use to support me
and also get all their customer
responsibility matrix? So that's kind of
the question in a nutshell, just phrased
a little bit of a different way. Um,
Ryan, what's your take? Because my take
would be the MSSP should incorporate
based on the tech sector that they're
using into the customer responsibility
matrix that they give you company ABC in
this example. So you don't have to go
hunt down because here's the thing, you
don't know what features and services
they're using of those products per se.
So that's my initial take on it. Ryan,
agreement, disagreement? What do you
think? Yeah, ultimately the the MSSP
should be kind of that that synthesis
layer where they're taking everything
they know about the tools that they're
using and using that to build the shared
responsibility matrix they give to their
end client. So the the only uh factors
that you'd want to pay attention to is
whether there are any pass through
services being provided by a vendor uh
that the MSSP is leveraging that are not
being clearly delineated in your service
relationship. So for example, the
CrowdStrike Falcon platform itself that
that secure now uses um is a security
protection asset, right? Secure now
actively manages it on their end when
they when they deploy the agents and
deliver your services and also you know
crowdstrike has their Falcon complete
service
>> which is a fully managed detection and
response service of its own. So I would
want to know how much or how little of
the available services that secure now
this MSSP is using from CrowdStrike. Are
they staffing their own sock? Did they
outsource that and things of that
nature? Because ultimately there needs
to be a direct line of responsibility to
how the requirements are being met and
all these other things. So,
>> you just want to make sure that you
don't overlook relationships that could
put you in a situation where on
assessment day there's no one in the
room who can intelligently speak to how
the sausage gets made.
>> That's a great that's a great clarifying
point. The other thing on top of it is
if these systems are processing,
storing, and transmitting CUI, one thing
that doesn't show up on customer
responsibility matrix is is this thing
fed ramp or not, right? Does it meet the
minimum requirements of moderate or
equivalent? So there is still probably a
level of due diligence worth asking your
MSSP, but to Ryan's point, they should
synthesize that information and serve
that to you or they're not exactly being
probably the best partner in that,
right? Because if you have to go hunt
for all the tools, you still have to go
back to them and say, "How are you using
these tools?" And, you know, they should
just kind of correlate all that for you.
So, um, we are at time. Uh, Jacob is on
a plane somewhere, hopefully headed back
home at this point. Uh, we're about to
get like a gajillion inches of snow here
in the south. So, we're going to go uh
test the generator to make sure that
we're all going to be okay and warm. Um,
for those that tuned in, thanks for
jumping on today. We didn't get to your
question. We're going to try and answer
it next week. Um, Ryan, it's been a
pleasure as always, my friend. I miss
talking to you. We'll talk more once
CMMC phase 2 starts, maybe. Um, and uh,
with that, we bid you all do, my
friends. Have a great weekend.
>> Bye all.
>> See you.
