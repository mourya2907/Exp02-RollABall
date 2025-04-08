# Exp02-RollABall
### AIM :
To develop a 3D application for RollABall in unity.
### ALGORITHM :
~~~
STEP 1 :
Create a new project.
STEP 2 :
Click Heirarchy -> 3D object -> Select the plane -> 3DObject -> Sphere.
STEP 3 :
Define the physics properties of the surfcae ( rigidbody)
STEP 4 :
Assets -> Create -> # Script
STEP 5 :
Create a folder name Coding and create a C# file to add the coding in it.
STEP 6 :
To add our C# Script file to our selected object, click on the C# Script file and drag it to our selected objects in the Hierarchy window nad run the application.
STEP 7 :
Stop
~~~
### PROGRAM :
### DEVELOPED BY : MOURYA . G
### REG NO : 212224230170
~~~
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class RollAball : MonoBehaviour
{
    // Start is called before the first frame update
    public float xforce = 5.0f, yforce = 200.0f, zforce = 5.0f;
    void Start()
    {


    }

    // Update is called once per frame
    void Update()
    {
        float x = 0.0f, y = 0.0f, z = 0.0f;
        if (Input.GetKey(KeyCode.A))
        {
            x = x - xforce;
        }
        if (Input.GetKey(KeyCode.D))
        {
            x = x + xforce;
        }
        if (Input.GetKey(KeyCode.W))
        {
            z = z + zforce;
        }
        if (Input.GetKey(KeyCode.S))
        {
            z = z - zforce;
        }
        if (Input.GetKeyDown(KeyCode.Space))
        {
            y = yforce;
        }
        GetComponent<Rigidbody>().AddForce(x, y, z);

    }
}
~~~
### OUTPUT : 
![309770903-334786f8-c8b5-4509-801d-cb405e3aa80b](https://github.com/user-attachments/assets/4efd8ddc-249e-462f-a20f-b242be6d91c1)
### RESULT :
Thus a 3D application for RollABall objects in unity is developed successfully.


