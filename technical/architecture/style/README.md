# Architectural Style

At the time of writing, we are focused on delivering the platform to a Beta audience.

The non-functional requirements for this deliverable are not as strict as they will be for the final FutureNHS platform, so concerns such as disaster recovery, observability, high scalability and performance are not as front an centre as they will be at the finish line.

As an added complexity, the platform is intended to be as pick-up-and-play as possible to assure ease of adoption for those who may wish to host something similar.  To this end, we consider the Beta timeframe to be the perfect opportunity for us to architect a solution that relies on a scale-up strategy (with minimal points of failure) to deliver the required scale/performance needed.  

For those who wish to take the platform into an environment with requirements that cannot be met by this approach, a scale-out alternative will come out of the production delivery to the FutureNHS team.  Undoubtedly more complex in terms of deployment, management and what good governance looks like, we assume anyone with such an audience would already have appropriate strategies and technical skills at hand to manage the added complexity of such.

## History of the Project

This is not the first attempt to deliver on our vision.  

Originally, we attempted to build a full on Microservice architecture right from the get-go but ultimately failed under the weight of (what in retrospect should be thought of as) *unnecessary* technical complexity brought about by demanding non-functional requirements, a lack of appreciation for the importance of iteratively identifying our logical service boundaries and the paralysing burden of trying to learn/adopt too much 'new stuff'.  

We always aim to learn from our *mistakes* and this time around, we want to be laser focused on delivering features we can get in front of our user base as soon as possible to elicit their valuable feedback for key functional areas, and to use such learnings to drive our decision making.  In order to do so, we have accepted that we need to kick some of the more technical concerns down the road, and the way we have done so is to relax the non-functional requirements for the Beta timeframe.

This approach certainly makes it easier to look at the adoption of existing open-sourced software to which we can contribute.  Out-of-the-box is the Beta mantra, and we aim to keep custom development to a minimum.  In the FutureNHS' case, we accept that out-of-the-box is unlikely to meet all our non-functional and functional requirements, and will thus look to contribute to these projects to make them more reliable, scalable, performant and automatically deployable to cloud infrastructure etc.

Post Beta, once we have a functioning platform adding real value to our users, we will be able to benchmark it accurately and then take a view as to any technical rework needed to take us towards meeting our production goals.  It won't be a big-bang situation so we will be able to manage the on-boarding of new users and platform functions in line with any work needed to productionise the platform and make it available to all.

## Our Evolving Architecture

[The Scale-Up Approach](scale-up.md)

[The Scale-Out Approach](scale-out.md)