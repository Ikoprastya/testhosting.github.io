<?php 
//koneksi database
	$server = "localhost";
	$user = "root";
	$pass = "";
	$database = "dblatihan";

	$koneksi = mysqli_connect($server, $user, $pass, $database)or die (mysqli_error($koneksi));

	
	//save data
	if(isset($_POST['bsimpan'])){

		//Save or Edit data
		if ($_GET['hal'] == "edit") {
			//for save data after edit
			$edit = mysqli_query($koneksi, " UPDATE tmhs set 
				contact = '$_POST[pcontact]',
				charName = '$_POST[pchar]',
				weapon = '$_POST[pweap]',
				server = '$_POST[pserver]'
				WHERE angka = '$_GET[id]'
				");

			if($edit){
				echo 
				"<script>
					alert('Edit Data Valid!');
					document.location = 'index.php';
				</script>";
			} else {
				echo 
				"<script>
					alert('Edit Data Invalid');
					document.location = 'index.php';
				</script>";
			}		

		} else {
			//save data
			$simpan = mysqli_query($koneksi, "INSERT INTO tmhs (contact, charName, weapon, server) 
				VALUES (
					'$_POST[pcontact]',
					'$_POST[pchar]',
					'$_POST[pweap]',
					'$_POST[pserver]')
				");

			if($simpan){
				echo 
				"<script>
					alert('Save Data Valid!');
					document.location = 'index.php';
				</script>";
			} else {
				echo 
				"<script>
					alert('Save Data Invalid');
					document.location = 'index.php';
				</script>";
			}		
		}
	}

	//Edit & Delete data
	if (isset($_GET['hal'])) {
		if ($_GET['hal'] == "edit") {
			$tampil = mysqli_query($koneksi,"SELECT * FROM tmhs WHERE angka = 
				'$_GET[id]' ");
			$data = mysqli_fetch_array($tampil);
			if($data){
				$vcontact = $data['contact'];
				$vcharName = $data['charName'];
				$vweapon = $data['weapon'];
				$vserver = $data['server'];
			}
		} else if($_GET['hal'] == "hapus"){
			$hapus = mysqli_query($koneksi, "DELETE FROM tmhs WHERE angka = '$_GET[id]' ");
			if($hapus){
				echo 
				"<script>
					alert('Delete Data Success. Thank You For Participation');
					document.location = 'index.php';
				</script>";
			}

		}
	}




 ?>

<!DOCTYPE html>
<html>
<head>
	<title>Trade Account Game</title>
	<link rel="stylesheet" type="text/css" href="css/bootstrap.min.css">
</head>
<body class="bg-secondary">
<div class="container">

		<h1 class="text-center mt-3 text-dark">Welcome to The Platform</h1>
		<h2 class="text-center mt-1 text-dark">Trade Account Genshin Impact</h2>


		<!-- Card Form Input Data -->
		<div class="card mt-5">
		  <div class="card-header bg-primary text-white">
		    INPUT TRADE ACCOUNT
		  </div>
		  <div class="card-body">
			<form method="post" action="">
	
				<div class="form-grup mt-1">
					<label>Contact</label>
					<input type="text" name="pcontact" value="<?=@$vcontact?>" class="form-control mt-2" placeholder="Input Your Contact Here! Like a Tiktok ex:@newaccount" required>
				</div>

				<div class="form-grup mt-1">
					<label>Character</label>
					<textarea class="form-control mt-2" name="pchar" placeholder="Input Your Character Here!"><?=@$vcharName?></textarea>
				</div>

				<div class="form-grup mt-1">
					<label>Weapon</label>
					<textarea class="form-control mt-2" name="pweap" placeholder="Input Your Weapon Here!"><?=@$vweapon?></textarea>
				</div>

				<div class="form-grup mt-1">
					<label>Server</label>
					<select class="form-control mt-2" name="pserver">
						<option value="<?=@$vserver?>"><?=@$vserver?></option>
						<option value="America">America</option>
						<option value="Europe">Europe</option>
						<option value="Asia">Asia</option>
						<option value="TW-HK-MO">TW-HK-MO</option>
					</select>
				</div>

				<button type="Submit" class="btn btn-success mt-3" name="bsimpan">Save</button>
				<a href="index.php" type="Reset" class="btn btn-danger mt-3" name="breset">Reset</a>
				
			</form>		  
		  </div>
		</div>
		<!-- Card Form -->

		<!-- Card Table Output Data -->
		<div class="card mt-5">
		  <div class="card-header bg-success text-white">
		    IF YOU WANT CONTACT THE PERSON!!!
		  </div>
		  <div class="card-body">
				  
				<table class="table table-bordered table-striped">
					<tr>
						<th>No.</th>
						<th class="text-center">Contact</th>
						<th class="text-center">Character</th>
						<th class="text-center">Weapon</th>
						<th class="text-center">Server</th>
						<th class="text-center">Action</th>
					</tr>
					<?php 
						$nomor = 1;
						$tampil = mysqli_query($koneksi, "SELECT * from tmhs order by angka desc");
						while ($data = mysqli_fetch_array($tampil)) :
						
					 ?>
					<tr>
						<td><?=$nomor++?></td>
						<td><?=$data['contact']?></td>
						<td><?=$data['charName']?></td>
						<td><?=$data['weapon']?></td>
						<td class="text-center"><?=$data['server']?></td>
						<!-- Edit & Delete data -->
						<td>
							<a href="index.php?hal=edit&id=<?=$data['angka']?>" class="btn btn-warning" name="bedit">EDIT</a>
							<a href="index.php?hal=hapus&id=<?=$data['angka']?>" onclick="return confirm('Do You Want To Delete?!')" class="btn btn-danger" name="bdelete">DELET</a>
						</td>
					</tr>

					<?php endwhile;?>
				</table>



		  </div>
		</div>
		<!-- Card Table -->



</div>


<script type="text/javascript" src="js/bootstrap.min.js"></script>
</body>
</html>