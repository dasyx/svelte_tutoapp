<script>
    const user = {
        firstName   : 'John',
        lastName : 'Doe',
        imageUrl : 'https://picsum.photos/200/300'
    };
    function getUser(user) {
        return user.firstName + ' ' + user.lastName;
    }
</script>

<h1>Hello {getUser(user)}</h1>
<img src={user.imageUrl} alt="sample" />