<div className='rooms-styles'>
    {rooms.length === 0 && <p>This server is missing rooms!! WERE GOING TO DIEEE!!</p>}
        <div>
            {rooms.length > 0 && rooms.map((roomBtn)=><button onClick={()=>{props.dispatch(changeRoom(roomBtn.roomName))}}>{roomBtn.roomName}</button>)}
         </div>
 </div>