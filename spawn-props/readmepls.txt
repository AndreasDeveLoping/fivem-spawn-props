How to place your prop

Citizen.CreateThread(function()
	Citizen.Wait(0)	
    local HashKey = GetHashKey("")                       ##put prop here
	local SpawnObject1 = CreateObject(HashKey, 0, 0, 0)  ##put coordinates here
	PlaceObjectOnGroundProperly(SpawnObject1)
	FreezeEntityPosition(SpawnObject1, true)             ##if you want your prop dont move put this true
	SetEntityHeading(SpawnObject1, 0.0)                  ##change prop heading
end)

change "SpawnObject1" this when you want place second prop like this

Citizen.CreateThread(function()
	Citizen.Wait(0)	
    local HashKey = GetHashKey("")
	local SpawnObject2 = CreateObject(HashKey, 0, 0, 0)
	PlaceObjectOnGroundProperly(SpawnObject2)
	FreezeEntityPosition(SpawnObject2, true)
	SetEntityHeading(SpawnObject2, 0.0)
end)

if you any problems text me:fivemdevfin@gmail.com