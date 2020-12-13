@startuml

Hero -> Princess: Talk
Princess -> CheckPoint: MoveTo
CheckPoint -> CheckPoint: starEvent
CheckPoint -> Hero: sendReward
Hero -> Princess: shareReward
Princess -> CheckPoint: isLastCheckpoint?
CheckPoint -> Princess: False:assignNextCheckPoint
Princess -> Hero: Talk, confirmAndContinue
Princess -> CheckPoint: MoveTo
CheckPoint -> SpawnPoint: summonSpawns
SpawnPoint -> Spawn: summonMinion
Spawn -> Princess: MoveTo
Princess -> Princess: setIsUnderAttack=True
Princess -> Princess: holdPosition
Princess -> Princess: canAttack?
Princess -> Princess: True:attackClosestSpawn
Princess -> Spawn: attackClosestTarget
Spawn -> Hero: askDistance
Hero -> Spawn: getDistance
Spawn -> Princess: askDistance
Princess -> Spawn: getDistance
Spawn -> Spawn: assigngTarget
Spawn -> Target: moveToAttackRange
Target -> Spawn: isInAttackRange
Spawn -> Spawn: StartAttack
Spawn -> Target: attack!
Target -> Target: hitSuccessful?
Target -> Target: reduceLifeFromAttack
Target -> Target: isAlive?
Target -> Target: False:PlayDeadAnimationAndEndGame
Target -> Spawn: True:ContinueUntilDead
Hero -> Spawn: attack
Princess -> Spawn: attack
Spawn -> Spawn: hitSuccessful?
Spawn -> Spawn: reduceLifeFromAttack
Spawn -> Spawn: isAlive?
Spawn -> Spawn: True:knockBack
Spawn -> Spawn: assigngTarget
Spawn -> Spawn: False:Die
Spawn -> Princess: NotifyDeath
Princess -> Princess: isThereAnySpawnLeft
Princess -> Princess: False:setIsUnderAttack=False
Princess -> CheckPoint: EndEvent

@enduml
