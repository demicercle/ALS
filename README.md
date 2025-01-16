# ALS

AnimMan
- GrabActor(newGrabbable)
- DropActor()
- EquipWeapon(newWeapon)
- DropWeapon()
- SetWeaponInHand(value)

Slot
- SlotActor(newActor)


OR

GrabbableComponent
> OnTick:
	> Attached?
		> Disable Collision
		> Disable Physics
	> Not Attached
		> Enable Collision
		> Enable Physics

SlotComponent
> AllowLeftHand
> AllowRightHand
> GetAttachedActor
> AttachActor(grabbable)

AnimMan
- WeaponSlot:SlotComponent
- 