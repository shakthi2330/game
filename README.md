using UnityEngine;
using System.Collections;

public class cube : MonoBehaviour {

	// Use this for initialization
	void Start () {
	
	}
	
	// Update is called once per frame
	void Update ()
    {
        transform.Translate(5f * Input.GetAxis("Horizontal") * Time.deltaTime, 0f, 5f * Input.GetAxis("Vertical") * Time.deltaTime);	
		transform.Rotate (0f,50f * Input.GetAxis ("Mouse X") * Time.deltaTime,0f);

}
}
