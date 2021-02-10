---  
id: MLAPI.NetworkingManager.ConnectionApprovedDelegate  
title: MLAPI.NetworkingManager.ConnectionApprovedDelegate  
---

<div class="markdown level0 summary" markdown="1">

Delegate type called when connection has been approved. This only has to
be set on the server.

</div>

<div class="markdown level0 conceptual" markdown="1">

</div>

##### **Namespace**: System.Dynamic.ExpandoObject

##### **Assembly**: MLAPI.dll

##### Syntax [MLAPI_NetworkingManager_ConnectionApprovedDelegate_syntax]

    public delegate void ConnectionApprovedDelegate(bool createPlayerObject, ulong? playerPrefabHash, bool approved, Vector3? position, Quaternion? rotation);

##### Parameters [parameters]

| Type                                      | Name                 | Description                                                                                                                                            |
|-------------------------------------------|----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| System.Boolean                            | \*createPlayerObject | If true, a player object will be created. Otherwise the client will have no object.                                                                    |
| System.Nullable\<System.UInt64\>          | \*playerPrefabHash   | The prefabHash to use for the client. If createPlayerObject is false, this is ignored. If playerPrefabHash is null, the default player prefab is used. |
| System.Boolean                            | \*approved           | Whether or not the client was approved                                                                                                                 |
| System.Nullable\<UnityEngine.Vector3\>    | \*position           | The position to spawn the client at. If null, the prefab position is used.                                                                             |
| System.Nullable\<UnityEngine.Quaternion\> | \*rotation           | The rotation to spawn the client with. If null, the prefab position is used.                                                                           |